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
        <div class="choose-kyan margin-top-section">
            <div class="container">
                <div class="titl-note d-flex justify-content-between align-items-center">
                    <div class="animation-top-Arrow d-flex justify-content-start align-items-center gap-4">
                        <p class="paragraph-sec w-50 text-end">نحن نهتم بأدق التفاصيل لضمان تجربة فريدة لطفلك تجمع بين
                            المتعة والتعلم
                            والأمان</p>
                        <div class="Arrow">
                            <Arrow />
                        </div>
                    </div>
                    <div class="mini-title-sec text-end">
                        <h5>لماذا تختار كيان؟</h5>
                        <h1 class="title">مميزات تجعلنا <span class="span-title">الأفضل</span> </h1>
                    </div>
                </div>
                <div class="row mt-5 flex-row-reverse">
                    <div class="col-lg-3 col-md-6 col-sm-12">
                        <div class="mask mask-1">
                            <img src="/box-1.webp" alt="" class="image-box">
                        </div>
                    </div>
                    <div class="col-lg-3 col-md-6 col-sm-12">
                        <div class="mask mask-2">
                            <img src="/box-2.webp" alt="" class="image-box">
                        </div>
                    </div>
                    <div class="col-lg-3 col-md-6 col-sm-12">
                        <div class="mask mask-3">
                            <img src="/box-3.webp" alt="" class="image-box">
                        </div>
                    </div>
                    <div class="col-lg-3 col-md-6 col-sm-12">
                        <div class="mask mask-4">
                            <img src="/box-4.webp" alt="" class="image-box">
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
<style scoped>
.section-one {
    background: linear-gradient(180deg, #fafdff 14.728%, #c3eaf9);
    top: -40px;
    min-height: 90vh;
    /* min-height: calc(90vh - 80px); */
    /* min-height: 100vh; */
}

.image img {
    max-width: 100%;
}

.wave {
    bottom: -90px;
    left: 0;
    width: 100%;
}

.wave svg path {
    /* width: 100%; */
    height: auto;
    display: block;

}

@media (max-width: 767px) {
    .section-one {
        min-height: auto;
        /* ارتفاع طبيعي حسب المحتوى */
        margin-top: 100px;
    }

    .row.align-items-center {
        flex-direction: column-reverse;
        /* الصورة تحت النص */
        text-align: center;
        /* النص في النص بدل text-end */
    }

    .details.text-end {
        text-align: center;
        margin-bottom: 20px;
    }

    .wave {
        bottom: -50px;
    }

    .title {
        font-size: 1.6rem;
    }

    .span-title {
        display: block;
    }

    .paragraph-sec {
        font-size: 0.95rem;
        line-height: 1.5rem;
    }
}

/* ////////////// sec chooose */
.mask {
    width: 200px;
    height: 200px;
    overflow: hidden;
    position: relative;
}

.mask-1 img {
    -webkit-mask-image: url('/mask-1.svg');
    mask-image: url('/mask-1.svg');
}

.mask-2 img {
    -webkit-mask-image: url('/mask-2.svg');
    mask-image: url('/mask-2.svg');
}

.mask-3 img {
    -webkit-mask-image: url('/mask-3.svg');
    mask-image: url('/mask-3.svg');
}

.mask-4 img {
    -webkit-mask-image: url('/mask-4.svg');
    mask-image: url('/mask-4.svg');
}

.image-box {
    width: 100%;
    height: 100%;
    object-fit: cover;
}
</style>