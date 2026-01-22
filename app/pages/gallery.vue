<template>
    <div class="kids-gallery mt-5 py-5">
        <PagintaePage />

        <div class="d-flex mt-3 align-items-center justify-content-center">
            <div class="mini-title-sec text-center">
                <h5> معرض الصور</h5>
                <h1 class="title">
                    لحظات من <span class="span-title">كيان المستقبل</span>
                </h1>

            </div>
        </div>
        <!-- filtter -->
        <div class="d-flex mt-4 gap-2 mb-4 btns overflow-auto">
            <button v-for="cat in categories" :key="cat" @click="selectCategory(cat)"
                :class="[selectedCategory === cat ? 'activeBtn' : 'noActive']">
                {{ cat }}
            </button>
        </div>
        <!--sppiner  -->
        <div v-if="loading" class="text-center my-4">
            <div class="spinner-border text-primary" role="status">
                <span class="visually-hidden">Loading...</span>
            </div>
        </div>
        <!-- images -->
        <div v-else class="container">
            <div class="row g-4">
                <div v-for="item in filteredImages" :key="item.id" class="col-md-3 col-sm-12">
                    <div class="">
                        <img @click="selectedImage = item.src" style="cursor: pointer;" :src="item.src"
                            class="card-img-top rounded-4" :alt="item.alt" />
                    </div>
                </div>
            </div>
        </div>

        <div v-if="selectedImage" class="lightbox" @click="selectedImage = null">
            <img :src="selectedImage" class="lightbox-img" />
        </div>
        <!-- contact-->
        <contact />
    </div>

</template>

<script setup>
definePageMeta({
    title: "معرض الصور"
})
const categories = ['المرافق', 'الفعاليات', 'الفنون', 'الأنشطة', 'الكل']
const images = [
    { id: 1, src: '/img-1.webp', alt: 'kids 1', category: 'الأنشطة' },
    { id: 2, src: '/img-2.webp', alt: 'kids 2', category: 'الفنون' },
    { id: 3, src: '/img-3.webp', alt: 'kids 3', category: 'الفعاليات' },
    { id: 5, src: '/img-4.webp', alt: 'kids 4', category: 'المرافق' },
    { id: 6, src: '/img-5.webp', alt: 'kids 5', category: 'الأنشطة' },
    { id: 4, src: '/img-3.webp', alt: 'kids 3', category: 'الفعاليات' },
    { id: 7, src: '/img-6.webp', alt: 'kids 6', category: 'الفنون' },
    { id: 8, src: '/img-6.webp', alt: 'kids 6', category: 'الفنون' },
]

const selectedImage = ref(null);

const loading = ref(false)
function selectCategory(cat) {
    selectedCategory.value = cat
    loading.value = true
    setTimeout(() => {
        loading.value = false
    }, 500) // 500ms أو أي وقت تحبه
}
const selectedCategory = ref('الكل')

const filteredImages = computed(() => {
    if (selectedCategory.value === 'الكل') return images
    return images.filter(img => img.category === selectedCategory.value)
})
</script>

<style>
.kids-gallery img {
    max-height: 200px;
    object-fit: cover;
}

.btns {
    overflow-x: auto;
    scroll-behavior: smooth;
    -webkit-overflow-scrolling: touch;
    justify-content: center;
    padding: 4px;
}

.btns::-webkit-scrollbar {
    display: none;
}

.activeBtn {
    background: linear-gradient(to right, #1aaee6, #0d607f);
    color: white;
    border: none;
    padding: 2px 20px;
    border-radius: 20px;
    cursor: pointer;
}

.noActive {
    background-color: rgb(255 255 255 / 1);
    color: black;
    padding: 2px 20px;
    border-radius: 20px;
    border: none;
    box-shadow: 0px 2px 5px rgba(0, 0, 0, 0.1);
    cursor: pointer;
}

.noActive:hover {
    background-color: #ccc;
}

.lightbox {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: rgba(0, 0, 0, 0.8);
    display: flex;
    justify-content: center;
    align-items: center;
    z-index: 1000;
    cursor: zoom-out;
}

.lightbox-img {
    max-width: 100%;
    max-height: 90%;
    border-radius: 10px;
}

@media (max-width: 768px) {
    .btns {
        flex-wrap: nowrap;
        gap: 10px;
        justify-content: left;
    }

    .btns button {
        flex: 0 0 auto;
    }
}
</style>