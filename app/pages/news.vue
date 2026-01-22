<template>
    <div class="news mt-3 pt-5">
        <PagintaePage />
        <div class="titl-sec">
            <div class="container">
                <div class="row justify-content-center mt-4">
                    <div class="col-lg-7 col-md-10 col-sm-12">
                        <div class="mini-title-sec text-center">
                            <h5> خدمات جديدة</h5>
                            <h1 class="title">
                                جديدنا
                            </h1>
                            <p class="mt-3 fs-5">
                                في كيان المستقبل، نؤمن بأن كل طفل يحمل في داخله موهبة تستحق الاكتشاف، ونسعى لتقديم خدمات
                                جديدة تُلهم
                                عقولهم وتنمّي مهاراتهم
                            </p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class="bg-color-section">
            <WaveUp />
            <div class="container py-5">
                <div class="row gap-2 justify-content-center">
                    <div class="col-lg-5 col-md-6 col-sm-12">
                        <div
                            class="box-new m rounded-3 bg-white text-center d-flex flex-column justify-content-center align-items-center h-100">
                            <h1 class="title fs-4">خدمة متابعة ما بعد المدرسة</h1>
                            <p class="p-design fs-5">
                                في مركز كيان المستقبل هدفنا أن يصبح التعلم متعة، والتفوق عادة.
                            </p>
                            <div class="btn-box">
                                <button style="background: linear-gradient(135deg, #cc1fa5, #7f1469)"
                                    class="rounded-5 px-4 py-2 text-white fw-bold btn-design">
                                    عرض تفاصيل الخدمه
                                </button>
                            </div>
                        </div>
                    </div>
                    <div class="col-lg-5 col-md-6 col-sm-12">
                        <div
                            class="box-new rounded-3 bg-white text-center d-flex flex-column justify-content-center align-items-center h-100">
                            <h1 class="title fs-4">مسارات تعليم اللغات</h1>
                            <p class="p-design fs-5">
                                نفتح أبواب العالم أمام أطفالكم مع دورات تقدَّم بأساليب شيّقة على أيدي الخبراء
                            </p>
                            <div class="btn-box">
                                <button style="background: var(--main-color);"
                                    class="rounded-5 px-4 py-2 text-white fw-bold btn-design">
                                    عرض تفاصيل الخدمه
                                </button>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            <div class="wave-rotate">
                <WaveDown />
            </div>
        </div>
        <contact />
    </div>
</template>
<script setup>
import WaveDown from '~/components/icons/waveDown.vue';
import WaveUp from '~/components/icons/waveUp.vue';

definePageMeta({
    title: " جديدنا ",
});
</script>

<style scoped>
.box-new {
    min-height: 300px;
    display: flex;
    align-items: center;
    flex-direction: column;
}

.p-design {
    color: #ccc
}

.btn-design {
    outline: none;
    border: none;
}
</style>