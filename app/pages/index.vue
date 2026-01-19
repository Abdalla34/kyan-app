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
        <!-- round section in center -->
        <div class="round-sec mb-5 ">
            <WaveUp />
            <div class="container p-5">
                <div class="mini-title-sec mb-4 text-center">
                    <h5>لماذا تختار كيان؟</h5>
                    <h1 class="title">
                        أركان تعليمية أركان تعليمية <span class="span-title">متطورة</span>
                    </h1>
                </div>
                <div class="row">
                    <div class="swiper mySwiper">
                        <div class="swiper-wrapper">

                            <div class="swiper-slide">
                                <div class="img-circle p-1 d-flex align-items-center justify-content-center color-1">
                                    <img src="/arts-corner.webp" alt="">
                                </div>
                            </div>

                            <div class="swiper-slide">
                                <div class="img-circle p-1 d-flex align-items-center justify-content-center color-2">
                                    <img src="/cooking-corner.webp" alt="">
                                </div>
                            </div>

                            <div class="swiper-slide">
                                <div class="img-circle p-1 d-flex align-items-center justify-content-center color-3">
                                    <img src="/corner-theater.webp" alt="">
                                </div>
                            </div>

                            <div class="swiper-slide">
                                <div class="img-circle p-1 d-flex align-items-center justify-content-center color-4">
                                    <img src="/learning-corner.webp" alt="">
                                </div>
                            </div>

                            <div class="swiper-slide">
                                <div class="img-circle p-1 d-flex align-items-center justify-content-center color-5">
                                    <img src="/ports-club.webp" alt="">
                                </div>
                            </div>

                            <div class="swiper-slide">
                                <div class="img-circle p-1 d-flex align-items-center justify-content-center color-6">
                                    <img src="/skills-corner.webp" alt="">
                                </div>
                            </div>

                        </div>


                        <!-- arrows -->
                        <div class="swiper-button-next"></div>
                        <div class="swiper-button-prev"></div>
                    </div>
                </div>
            </div>
            <div class="wave-rotate">
                <waveDown />
            </div>
        </div>
    </div>
</template>
<script setup>
import Swiper from 'swiper/bundle'
import 'swiper/css'
import 'swiper/css/navigation'
import Wave from '~/components/icons/wave.vue'
import WaveDown from '~/components/icons/waveDown.vue'
import WaveUp from '~/components/icons/waveUp.vue'
onMounted(() => {
    new Swiper('.mySwiper', {
        slidesPerView: 4,
        spaceBetween: 20,
        loop: true,
        autoplay: {
            delay: 2500,
            disableOnInteraction: false,
        },
        navigation: {
            nextEl: '.swiper-button-next',
            prevEl: '.swiper-button-prev',
        },
        breakpoints: {
            0: {
                slidesPerView: 1,
            },
            576: {
                slidesPerView: 2,
            },
            768: {
                slidesPerView: 3,
            },
            992: {
                slidesPerView: 4,
            },
        },
    })
})

</script>

<style scoped>
@import "assets/pages/section-main.css";
/*  sec chooose */
@import "assets/pages/choosing-kayan.css";

.round-sec {
    background: linear-gradient(270deg, #fdecf8, #edf8fd);
}

.swiper {
    width: 100%;
    padding: 20px 0;
}

.swiper-slide img {
    width: 100%;
    height: 250px;
    object-fit: cover;
    border-radius: 12px;
}

.img-circle {
    width: 250px;
    height: 250px;
    border-radius: 50%;
    margin: auto;
}

.img-circle img {
    width: 100%;
    height: 100%;
    border-radius: 50%;
    object-fit: cover;
}

/* Borders colors for each image */
.color-1 {
    background: conic-gradient(#00bfff 0% 25%, #00ffff 25% 50%, #0077ff 50% 75%, #00ffaa 75% 100%);
    /* border-width: ; */
}

.color-2 {
    background: conic-gradient(#ff7f50 0% 25%, #ff4500 25% 50%, #ff6347 50% 75%, #ffa07a 75% 100%);
    /* border-width: ; */
}

.color-3 {
    background: conic-gradient(#7b68ee 0% 25%, #6a5acd 25% 50%, #9370db 50% 75%, #8a2be2 75% 100%);
    /* border-width: ; */
}

.color-4 {
    background: conic-gradient(#32cd32 0% 25%, #00ff00 25% 50%, #228b22 50% 75%, #7fff00 75% 100%);
    /* border-width: ; */
}

.color-5 {
    background: conic-gradient(#ff69b4 0% 25%, #ff1493 25% 50%, #ffb6c1 50% 75%, #ff00ff 75% 100%);
    /* border-width: ; */
}

.color-6 {
    background: conic-gradient(#ffa500 0% 25%, #ff8c00 25% 50%, #ffd700 50% 75%, #ff4500 75% 100%);
}
.wave-rotate{
    position: relative;
    transform: rotate(180deg);
}
</style>