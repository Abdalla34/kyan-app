<template>
    <div class="news mt-3 pt-5">
        <PagintaePage />
        <!-- first section -->
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
        <!-- boxes services -->
        <div class="bg-color-section">
            <WaveUp />
            <div class="container py-5">
                <div class="row gap-2 justify-content-center">
                    <div class="col-lg-5 col-md-6 col-sm-12">
                        <div
                            class="box-new m rounded-4 bg-white text-center d-flex flex-column justify-content-center align-items-center h-100">
                            <h1 class="title fs-4">خدمة متابعة ما بعد المدرسة</h1>
                            <p class="p-design fs-5">
                                في مركز كيان المستقبل هدفنا أن يصبح التعلم متعة، والتفوق عادة.
                            </p>
                            <div class="btn-box">
                                <NuxtLink
                                    style="background: linear-gradient(135deg, #cc1fa5, #7f1469); text-decoration: none;"
                                    class="rounded-5 px-4 py-2 hover text-white fw-bold btn-design">
                                    عرض تفاصيل الخدمه
                                </NuxtLink>
                            </div>
                        </div>
                    </div>
                    <div class="col-lg-5 col-md-6 col-sm-12">
                        <div
                            class="box-new rounded-4 bg-white text-center d-flex flex-column justify-content-center align-items-center h-100">
                            <h1 class="title fs-4">مسارات تعليم اللغات</h1>
                            <p class="p-design fs-5">
                                نفتح أبواب العالم أمام أطفالكم مع دورات تقدَّم بأساليب شيّقة على أيدي الخبراء
                            </p>
                            <div class="btn-box">
                                <NuxtLink to="#table-serv" style="background: var(--main-color); text-decoration: none;"
                                    class="rounded-5 px-4 py-2 hover text-white fw-bold btn-design">
                                    عرض تفاصيل الخدمه
                                </NuxtLink>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            <div class="wave-rotate">
                <WaveDown />
            </div>
        </div>
        <!-- table  -->
        <div class="table-serv" id="table-serv">
            <div class="container">
                <div class="serv-num p-3 mb-3 d-flex align-items-center justify-content-center">
                    <span class="title fs-5 fw-bold">1</span>
                </div>


                <div class="mini-title-sec mb-5 text-center">

                    <h1 class="title fs-3">
                        مسارات تعلم اللغات
                    </h1>
                    <p class="mt-3 fs-5 w-50 w-mobile mx-auto">
                        في كيان المستقبل، نؤمن بأن كل طفل يحمل في داخله موهبة تستحق الاكتشاف، ونسعى لتقديم خدمات
                        جديدة تُلهم
                        عقولهم وتنمّي مهاراتهم
                    </p>
                </div>

                <div class="row justify-content-center align-items-center">
                    <div class="col-lg-8">
                        <table class="table table-bordered table-hover text-center align-middle rounded-4">
                            <thead class="table-head">
                                <tr>
                                    <th scope="col">اللغة</th>
                                    <th scope="col">الأيام</th>
                                    <th scope="col">الوقت</th>
                                    <th scope="col">الوجبة</th>
                                </tr>
                            </thead>

                            <tbody>
                                <tr class="">
                                    <td>🇬🇧 الإنجليزية</td>
                                    <td>الأحد – الثلاثاء – الخميس</td>
                                    <td>من 3 إلى 4 عصرًا</td>
                                    <td>شاملة وجبة الغداء</td>
                                </tr>
                                <tr class="">
                                    <td>🇪🇸 الإسبانية</td>
                                    <td>الثلاثاء – الأربعاء</td>
                                    <td>من 1 ظهرًا إلى 3 عصرًا</td>
                                    <td>شاملة وجبة الغداء</td>
                                </tr>
                                <tr>
                                    <td>🇫🇷 الفرنسية</td>
                                    <td>الأحد – الاثنين</td>
                                    <td>من 1 ظهرًا إلى 3 عصرًا</td>
                                    <td>شاملة وجبة الغداء</td>
                                </tr>
                            </tbody>
                        </table>
                    </div>
                </div>
            </div>
        </div>
        <!-- services school -->
        <div class="serv-school mt-4">
            <div class="container">
                <div class="serv-num p-3 color-bg mb-3 d-flex align-items-center justify-content-center">
                    <span class="title text-color fs-5 fw-bold">2</span>
                </div>
                <div class="mini-title-sec mb-5 text-center">

                    <h1 class="title fs-3">
                        خدمة متابعة ما بعد المدرسة
                    </h1>
                    <p class="mt-3 fs-5 w-mobile w-50 mx-auto">
                        في خدمة متابعة ما بعد المدرسة فريقنا جاهز لمساعدة أطفالكم على تحقيق التفوق من خلال
                    </p>
                </div>
                <div class="box-serv py-4 rounded-5">
                    <div class="container">
                        <div class="row">
                            <div class="col-lg-12 col-sm-12">
                                <div class="mini-box m-3  bg-white rounded-4 text-end p-3 d-flex align-items-center justify-content-end">
                                    <h3 class="title fs-5">تنظيم ومراجعة يومية للدروس</h3>
                                </div>
                                <div class="mini-box m-3 bg-white rounded-4 p-3 d-flex align-items-center justify-content-end">
                                    <h3 class="title fs-5">إنجاز الواجبات بسرعة واحترافية</h3>
                                </div>
                                <div class="mini-box m-3 bg-white rounded-4 text-end p-3 d-flex align-items-center justify-content-end">
                                    <h3 class="title fs-5">تقديم دعم لمعالجة أي صعوبات تعليمية</h3>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div class="btn-contact d-flex justify-content-center mt-2">
                        <NuxtLink to="/contact" class="btn-link hover btn btn-primary rounded-5 px-4 py-2">
                            تواصل معنا للمزيد من التفاصيل والحجز
                        </NuxtLink>
                    </div>

                </div>
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
@import "assets/pages/new.css";

/* services 2 */


.btn-link {
    background-color: #128c7e;
    color: white;
    text-decoration: none;
}
</style>