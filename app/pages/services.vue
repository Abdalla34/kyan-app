<template>
    <div class="services mt-5 pt-5">
        <PagintaePage />
        <div class="round-sec mb-5">
            <WaveUp />

            <div class="container p-5">
                <div class="mini-title-sec mb-4 text-center">
                    <h5>جولة داخل المركز</h5>
                    <h1 class="title color-special">
                        أركان تعليمية <span class="span-title">متطورة</span>
                    </h1>
                </div>

                <div class="row justify-content-end g-4">
                    <div v-for="item in services" :key="item.id" class="col-lg-3 col-md-6 col-sm-12 box text-center"
                        @click="navigateTo(`/service/${item.id}`)">
                        <div class="img-circle mb-3" :class="item.color">
                            <img :src="item.image" :alt="item.title">
                        </div>

                        <h6 class="item-title">{{ item.title }}</h6>
                        <p class="item-desc">{{ item.desc }}</p>
                    </div>
                </div>
            </div>
            <Contact />
            <div class="wave-rotate">
                <WaveDown />
            </div>
        </div>
    </div>
</template>

<script setup>
const { services } = useServices();

definePageMeta({
    title: "أركان المركز"
})
</script>


<style scoped>
.box {
    transition: all ease-in-out 0.3s;
    cursor: pointer;
}

.box:hover {
    color: rgb(41, 233, 233);
    transform: scale(1.1);
}

.item-desc {
    font-size: 13px;
    color: #777;
    line-height: 1.6;
}
</style>