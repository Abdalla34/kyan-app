<template>
    <PagintaePage class="mt-5 pt-4" />
    <div class="blog bg-color-section">
        <div class="container py-4">
            <div class="d-flex mb-5 mb-mobile align-items-center justify-content-center">
                <div class="mini-title-sec text-center">
                    <h5> مقالات ونصائح</h5>
                    <h1 class="title">
                        المدونة
                    </h1>

                </div>
            </div>
            <div class="row row-mobile align-items-center justify-content-center">
                <!-- secion box mini -->
                <div class="col-lg-3 col-sm-12">
                    <!-- box search -->
                    <div class="box-side box-search p-3 py-4 bg-white rounded-4">
                        <h3 class="text-end fs-5 title">البحث</h3>
                        <div class="position-relative">
                            <input type="text" class="form-control ps-5 text-end" placeholder="...ابحث في المدونة">
                            <span class="position-absolute top-50 start-0 translate-middle-y ps-3 text-muted">
                                🔍
                            </span>
                        </div>
                    </div>
                    <!-- Categories -->
                    <div class="categories box-side p-3 py-4 bg-white rounded-4 mt-3">
                        <h3 class="text-end fs-5 title">التصنيفات</h3>
                        <p
                            class="mt-4 text-end text-hover d-flex align-items-center justify-content-between flex-row-reverse">
                            تربية الأطفال <span
                                class="circle-num p-1 d-flex align-items-center justify-content-center ">12</span>
                        </p>
                        <p
                            class="mt-2 text-end text-hover d-flex align-items-center justify-content-between flex-row-reverse">
                            التعليم المبكر <span
                                class="circle-num p-1 d-flex align-items-center justify-content-center ">6</span>
                        </p>
                        <p
                            class="mt-2 text-end text-hover d-flex align-items-center justify-content-between flex-row-reverse">
                            نصائح تربوية <span
                                class="circle-num p-1 d-flex align-items-center justify-content-center ">8</span>
                        </p>
                        <p
                            class="mt-2 text-end text-hover d-flex align-items-center justify-content-between flex-row-reverse">
                            تعليم اللغات <span
                                class="circle-num p-1 d-flex align-items-center justify-content-center ">10</span>
                        </p>
                        <p
                            class="mt-2 text-end text-hover d-flex align-items-center justify-content-between flex-row-reverse">
                            صحة الطفل <span
                                class="circle-num p-1 d-flex align-items-center justify-content-center ">11</span>
                        </p>
                        <p
                            class="mt-2 text-end text-hover d-flex align-items-center justify-content-between flex-row-reverse">
                            أنشطة منزلية <span
                                class="circle-num d-flex align-items-center justify-content-center p-1 ">3</span>
                        </p>
                    </div>
                    <!-- Latest articles -->
                    <div class="box-side mb-3 p-3 py-4 bg-white rounded-4 mt-3">
                        <h3 class="text-end fs-5 title">أحدث المقالات</h3>
                        <div class="d-flex mb-2 align-items-center justify-content-end gap-2"
                            v-for="article in articles.slice(0, 3)" :key="article">
                            <div>
                                <h1 class="title fs-6 text-end">{{ article.title }}</h1>
                                <p class="date text-end">{{ article.date }}</p>
                            </div>
                            <img class="img rounded-2" :src="article.img" alt="">
                        </div>
                    </div>
                </div>
                <div class="col-lg-8 col-md-8 col-sm-12">
                    <div class="row g-4">
                        <div class="col-lg-6 col-md-6 col-sm-12" v-for="blog in articles" :key="blog.id"
                            @click="navigateTo('/blogId')">
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
@import "assets/pages/blog.css";
</style>