<template>
    <PagintaePage class="mt-5 pt-4" />
    <div class="blog bg-color-section">
        <div class="container py-4">
            <div class="d-flex mb-5 align-items-center justify-content-center">
                <div class="mini-title-sec text-center">
                    <h5> مقالات ونصائح</h5>
                    <h1 class="title">
                        المدونة
                    </h1>

                </div>
            </div>
            <div class="row">
                <!-- secion box mini -->
                <div class="col-lg-3 col-sm-12"></div>
                <div class="col-lg-8 col-md-8 col-sm-12">
                    <div class="row g-4">
                        <div class="col-lg-6 col-md-6 col-sm-12" v-for="blog in articles" :key="blog.id">
                            <div class="card h-100 rounded-4 p-3 d-flex flex-columns">
                                <div class="image-wrapper mb-3">
                                    <img :src="blog.img" class="rounded-4 w-100" />
                                </div>
                                <h5 class="title mb-2 fs-5 text-end text-hover">
                                    {{ blog.title }}
                                </h5>
                                <p class="text-muted text-end mt-3" style="min-height: 60px">
                                    {{ blog.excerpt }}
                                </p>
                                <div class="mt-auto text-end d-flex align-items-center justify-content-between">
                                    <span class="badge bg-primary">اقرأ المزيد</span>
                                    <span>{{ blog.date }}</span>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class="wave-rotate">
            <WaveDown />
        </div>
    </div>
</template>
<script setup>
import WaveDown from '~/components/icons/waveDown.vue';

definePageMeta({
    title: " المدونه "
})

const { articles } = useServices();

</script>

<style scoped>
.cursor-pointer {
    cursor: pointer;
    border-bottom: 1px solid #ccc;
    flex-direction: row-reverse;
}

.cursor-pointer:last-child {
    border-bottom: none;
}

.card {
    cursor: pointer;
    border: none;
    box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
    transition: box-shadow 0.3s ease, transform 0.3s ease;
}

.card:hover {
    box-shadow: 0 8px 24px rgba(0, 0, 0, 0.15);
    transform: translateY(-4px);
}

.box-shadow {
    box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
}

.image-wrapper img {
    object-fit: cover;
    height: 180px;
}

.title-blog {
    font-size: 17px;
    color: var(--main-color-bg);
    font-weight: bold;
}

.filtter-item {
    background-color: rgb(243 245 247 / 1);
    cursor: pointer;
    font-size: 20px;
}

.filtter-item:hover {
    background-color: #ccc;
}

.text-hover:hover {
    color: var(--second-color-bg) !important;
}
</style>