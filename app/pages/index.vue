<script setup lang="ts">
import Arrow from '~/components/icons/Arrow.vue';

</script>

<template>
    <div class="main">
        <!-- image sec -->
        <div class="section-one position-relative d-flex align-items-center">
            <div class="container">
                <div class="row p-4 align-items-center">
                    <div class="col-lg-6 col-md-6 col-sm-12">
                        <div class="image animation-top">
                            <img src="/hero-left.webp" alt="">
                        </div>
                    </div>
                    <div class="col-lg-6 col-md-6 col-sm-12">
                        <div class="details text-end">
                            <div class="mini-title">
                                <h4>مركز كيان المستقبل لضيافة الأطفال</h4>
                                <h1 class="title fw-bold">خطوة بخطوة نأسس له <span class="span-title">مستقبل مشرق</span>
                                </h1>
                                <p class="paragraph-sec w-75">نساعد طفلك على اكتشاف مهاراته وتطوير قدراته في بيئة آمنة
                                    ومحفزة، لنصنع معاً جيلاً مبدعاً وواثقاً.</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            <div class="position-absolute wave">
                <IconsWave />
            </div>
        </div>
        <!-- choosing sec -->
        <div class="choose-kyan margin-top-section pt-5">
            <div class="container">
                <!-- Title Section -->
                <div class="titl-note d-flex justify-content-between align-items-center">
                    <div class="animation-top-Arrow d-flex justify-content-start align-items-center gap-4">
                        <p class="paragraph-sec w-50 text-end">
                            نحن نهتم بأدق التفاصيل لضمان تجربة فريدة لطفلك تجمع بين
                            المتعة والتعلم والأمان
                        </p>
                        <div class="Arrow">
                            <Arrow />
                        </div>
                    </div>

                    <div class="mini-title-sec text-end">
                        <h5>لماذا تختار كيان؟</h5>
                        <h1 class="title">
                            مميزات تجعلنا <span class="span-title">الأفضل</span>
                        </h1>
                    </div>
                </div>

                <!-- Boxes -->
                <div class="row mt-5 flex-row-reverse text-center">
                    <div class="col-lg-3 col-md-6 col-sm-12 box-item">
                        <div class="mask mask-1 mx-auto">
                            <img src="/box-1.webp" alt="" class="image-box">
                        </div>
                        <h4 class="title fs-5 mt-3">رعاية شاملة</h4>
                        <p class="p-imge">بيئة آمنة وصحية تضمن راحة طفلك واطمئنانك</p>
                    </div>

                    <div class="col-lg-3 col-md-6 col-sm-12 box-item">
                        <div class="mask mask-2 mx-auto">
                            <img src="/box-2.webp" alt="" class="image-box">
                        </div>
                        <h4 class="title fs-5 mt-3">تعليم ترفيهي</h4>
                        <p class="p-imge">مناهج تعليمية مبتكرة تمزج بين المتعة والفائدة</p>
                    </div>

                    <div class="col-lg-3 col-md-6 col-sm-12 box-item">
                        <div class="mask mask-3 mx-auto">
                            <img src="/box-3.webp" alt="" class="image-box">
                        </div>
                        <h4 class="title fs-5 mt-3">تنمية مهارات</h4>
                        <p class="p-imge">برامج متخصصة لتطوير القدرات الذهنية والحركية</p>
                    </div>

                    <div class="col-lg-3 col-md-6 col-sm-12 box-item">
                        <div class="mask mask-4 mx-auto">
                            <img src="/box-4.webp" alt="" class="image-box">
                        </div>
                        <h4 class="title fs-5 mt-3 ">تغذية صحية</h4>
                        <p class="p-imge">وجبات متوازنة ومتابعة دقيقة لصحة الطفل</p>
                    </div>
                </div>
            </div>
        </div>

    </div>
</template>
<style scoped>
@import "assets/pages/section-main.css";

/*  sec chooose */
@import "assets/pages/choosing-kayan.css";
</style>