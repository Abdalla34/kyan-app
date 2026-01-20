<template>
    <div class="about mt-5 pt-4">
        <PagintaePage />
        <div class="container pt-4">
            <div class="mini-title-sec text-center">
                <h5> تعرف علينا</h5>
                <h1 class="title">
                    عن مركز <span class="span-title">كيان المستقبل</span>
                </h1>
                <p class="mt-3">
                    نحن نؤمن بأن كل طفل يحمل في داخله بذرة التميز، ومهمتنا هي رعاية هذه البذرة لتنمو وتزهر
                </p>
            </div>
        </div>
        <div class="bg-color-section">
            <WaveUp />
            <div class="container p-5">
                <div class="row">
                    <div class="col-lg-6 col-md-6 col-sm-12">
                        <div class="mini-title-sec text-media text-end mt-3">
                            <h5> قصتنا</h5>
                            <h1 class="title">
                                رحلة نحو <span class="span-title"> التميز</span>
                            </h1>
                            <p class="mt-4 fs-6 fw-bold">
                                تأسس مركز كيان المستقبل برؤية واضحة تهدف إلى بناء جيل طموح يكون قاعدة أساسية لمستقبل
                                معرفي باهر ذو فكر مضيء وأهداف واضحة وطموحة.
                            </p>
                            <p class="mt-4 fs-6 fw-bold">
                                نحن نؤمن بأن السنوات الأولى من حياة الطفل هي الأكثر أهمية في تشكيل شخصيته ومستقبله، لذلك
                                نحرص على توفير بيئة آمنة ومحفزة تساعد الأطفال على اكتشاف قدراتهم وتطوير مهاراتهم.
                            </p>
                        </div>
                    </div>
                    <div class="col-lg-6 col-md-6 col-sm-12">
                        <img class="img rounded-4" src="/about.jpg" alt="">
                    </div>
                </div>
            </div>
            <div class="wave-rotate">
                <WaveDown />
            </div>
        </div>
        <div class="message">
            <div class="mini-title-sec text-media text-center mt-3">
                <h5> رؤيتنا ورسالتنا</h5>
                <h1 class="title color-special">
                    نبني المستقبل <span class="span-title"> معاً</span>
                </h1>

            </div>
            <div class="container">
                <div class="row mt-5">
                    <div class="col-lg-6 col-md-6 col-sm-12">
                        <div class="box-details mb-3 d-flex align-items-center flex-columns rounded-4 p-4">
                            <div class="icon" style="background-color: var(--main-color);">
                            </div>
                            <div class="text-details">
                                <h2 class="min-title text-end">رؤيتنا</h2>
                                <p class="fs-6 text-end mt-3">
                                    أن نكون المركز الرائد في ضيافة الأطفال بالمملكة، ونموذجًا يُحتذى به في الرعاية
                                    والتعليم لبناء جيل مبدع وواعٍ.
                                </p>
                            </div>
                        </div>
                    </div>
                    <div class="col-lg-6 col-md-6 col-sm-12">
                        <div class="box-details d-flex align-items-center flex-columns rounded-4 p-4">
                            <div class="icon" style="background-color: var(--main-color);"></div>
                            <div class="text-details">
                                <h2 class="min-title text-end">رسالتنا</h2>
                                <p class="fs-6 text-end mt-3">توفير بيئة آمنة ومحفزة تجمع بين الرعاية الشاملة والتعليم
                                    الترفيهي، مع
                                    التركيز على تنمية المهارات الذهنية والاجتماعية والحركية للأطفال.</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <!-- section contact -->
        <contact />
    </div>
</template>

<script setup>
import WaveDown from '~/components/icons/waveDown.vue'
import WaveUp from '~/components/icons/waveUp.vue'

definePageMeta({
    title: " عن كيان",
});
</script>
<style scoped>
.box-details {
    background-image: linear-gradient(to bottom right,
            #eaf8ff,
            #fde9f7);
    height: 300px;
}

@media(max-width:768px) {
    .text-media {
        text-align: center !important;
    }

    .text-media p {
        font-size: 12px !important;
    }
}
</style>>