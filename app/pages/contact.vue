<template>
    <PagintaePage class="mt-5 pt-4" />
    <div class="container mt-4">
        <div class="mini-title-sec text-center">
            <h5> تواصل معنا

            </h5>
            <h1 class="title">
                نحن هنا <span class="spa-title">لمساعدتك</span>
            </h1>
            <p>لديك استفسار أو ترغبين في تسجيل طفلك؟ تواصلي معنا وسنرد عليك في أقرب وقت</p>
        </div>
    </div>
    <div class="contact bg-color-section ">
        <WaveUp />

        <div class="container py-4">
            <div class="row justify-content-center">
                <!-- secion box mini -->
                <div class="col-lg-3 col-sm-12">
                    <!-- Categories -->
                    <div class="categories mb-3 box-side p-3 py-4 bg-white rounded-4 mt-3">
                        <h3 class="text-end fs-5 title mb-4">معلومات التواصل</h3>
                        <div class="box-contact rounded-3 mb-2 text-end p-2">
                            <span style="color:#ccc;">اتصلي بنا</span>
                            <h4 class="fs-6">0505996562</h4>
                        </div>
                        <div class="box-contact rounded-3 mb-2 text-end p-2">
                            <span style="color:#ccc;">واتساب</span>
                            <h4 class="fs-6">راسلينا الآن</h4>
                        </div>
                        <div class="box-contact rounded-3 mb-2 text-end p-2">
                            <span style="color:#ccc;">البريد الإلكتروني</span>
                            <h4 class="fs-6">info@futurekayan.com</h4>
                        </div>
                        <div class="box-contact rounded-3 mb-2 text-end p-2">
                            <span style="color:#ccc;">العنوان</span>
                            <h4 class="fs-6">
                                الرياض ، حي الرائد ، شارع عبدالعزيز الاحسائي</h4>
                        </div>
                    </div>

                </div>
                <div class="col-lg-8 col-sm-12">

                    <div class="form bg-white rounded-4">
                        <form class="p-4 rounded-4 shadow-sm bg-form" dir="rtl">
                            <!-- الاسم + الهاتف -->
                            <div class="row g-3 mb-3">
                                <div class="col-12 col-md-6">
                                    <label class="form-label">
                                        الاسم الكامل <span class="text-danger">*</span>
                                    </label>
                                    <input type="text" class="form-control rounded-pill input-color text-end"
                                        placeholder="أدخل اسمك الكامل" />
                                </div>

                                <div class="col-12 col-md-6">
                                    <label class="form-label">
                                        رقم الهاتف <span class="text-danger">*</span>
                                    </label>
                                    <input type="tel" class="form-control rounded-pill input-color text-end"
                                        placeholder="أدخل رقم الهاتف للتواصل" />
                                </div>
                            </div>


                            <!-- البريد + التاريخ -->
                            <div class="row g-3 mb-3">

                                <div class="col-md-12">
                                    <label class="form-label">البريد الإلكتروني</label>
                                    <input type="email" class="form-control rounded-pill input-color"
                                        placeholder="أدخل بريدك الإلكتروني" />
                                </div>
                            </div>

                            <!-- نوع الفعالية -->
                            <div class="mb-3">
                                <label class="form-label">نوع الفعالية</label>
                                <select class="form-select rounded-pill input-color">
                                    <option selected disabled>
                                        اختر نوع الفعالية (مؤتمر، معرض، حفل...)
                                    </option>
                                    <option>مؤتمر</option>
                                    <option>معرض</option>
                                    <option>حفل</option>
                                    <option>فعالية خاصة</option>
                                </select>
                            </div>

                            <!-- وصف الطلب -->
                            <div class="mb-4">
                                <label class="form-label">رسالتك *</label>
                                <textarea class="form-control rounded-4 input-color" rows="4"
                                    placeholder="اكتبي رسالتك هنا ..."></textarea>

                            </div>

                            <!-- زر الإرسال -->
                            <div class="text-center">
                                <button type="submit" class="btn btn-lg w-100 text-white btn-hover  rounded-pill"
                                    style="background: linear-gradient(135deg, #cc1fa5, #7f1469)">
                                    ارسال الرساله
                                </button>
                            </div>
                        </form>
                    </div>

                </div>
            </div>
            <div class="map-wrapper mt-4 rounded-4 overflow-hidden">
                <iframe src="https://www.google.com/maps?q=24.712901,46.636556&z=15&output=embed" width="100%"
                    height="400" style="border:0;" allowfullscreen="" loading="lazy"
                    referrerpolicy="no-referrer-when-downgrade">
                </iframe>
            </div>

        </div>
        <div class="wave-rotate">
            <WaveDown />
        </div>
    </div>
</template>
<script setup>
import WaveDown from '~/components/icons/waveDown.vue';
import WaveUp from '~/components/icons/waveUp.vue';

definePageMeta({
    title: "تواصل معنا "
})
</script>
<style scoped>
.box-contact {
    background-image: linear-gradient(to bottom right, #eaf8ff, #fde9f7);
    transition: all ease-in-out 0.3s;
    cursor: pointer;
}

.box-contact:hover {
    transform: scale(1.05);
    box-shadow: 0 8px 24px rgba(0, 0, 0, 0.1);
}
</style>