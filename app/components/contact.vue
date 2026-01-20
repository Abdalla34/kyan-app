<script setup lang="ts">
import WaveDown from './icons/waveDown.vue';
import WaveUp from './icons/waveUp.vue';
import IconsArrowBg from './icons/ArrowBg.vue';

</script>

<template>
  <div class="contact bg-color-section mt-5">
    <WaveUp />
    <div class="container p-4">
      <div class="row reverse justify-content-center align-items-center">
        <div class="col-lg-6 col-md-6 col-sm-12">
          <div class="form">
            <form class="p-4 rounded-4 shadow-sm bg-form" dir="rtl">
              <!-- الاسم + الهاتف -->
              <div class="row g-3 mb-3">
                <div class="col-12">
                  <label class="form-label">
                    الاسم الكامل <span class="text-danger">*</span>
                  </label>
                  <input type="text" class="form-control rounded-pill input-color" placeholder="أدخل اسمك الكامل" />
                </div>
              </div>

              <!-- البريد + التاريخ -->
              <div class="row g-3 mb-3">
                <div class="col-md-6">
                  <label class="form-label">
                    رقم الهاتف <span class="text-danger">*</span>
                  </label>
                  <input type="tel" class="form-control rounded-pill input-color"
                    placeholder="أدخل رقم الهاتف للتواصل" />
                </div>
                <div class="col-md-6">
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
                <label class="form-label">وصف مختصر للطلب</label>
                <textarea class="form-control rounded-4 input-color" rows="4"
                  placeholder="اكتب تفاصيل طلبك أو استفسارك"></textarea>
                <small class="text-muted "> يرجى إدخال الأحرف على الأقل </small>
              </div>

              <!-- زر الإرسال -->
              <div class="text-center">
                <button type="submit" class="btn btn-lg w-100 text-white btn-hover  rounded-pill"
                  style="background: linear-gradient(135deg, #cc1fa5, #7f1469)" ;>
                  سجلي الأن
                </button>
              </div>
            </form>
          </div>
        </div>
        <div class="col-lg-6 col-md-6 col-sm-12">
          <div class="mini-title-sec text-end">
            <h5>أنضمي الينا</h5>
            <h1 class="title color-special">
              هل أنتِ مستعدة لتسجيل طفلك؟
            </h1>
            <p class="fs-5 text-end">انضمي إلى عائلة كيان المستقبل ودعي طفلك يستمتع بتجربة فنية فريدة</p>
          </div>
          <div class="md-none">
            <IconsArrowBg />
          </div>
        </div>
      </div>
    </div>
    <div class="wave-rotate">
      <WaveDown />
    </div>
  </div>
</template>
<style scoped>
.bg-form {
  background: linear-gradient(180deg, hsla(0, 0%, 100%, .8), hsla(0, 0%, 100%, .2));
}

.input-color,
.input-color::placeholder {
  color: #ccc !important;
  text-align: right;
}



.btn-hover {
  transition: all ease-in-out 0.3s;
}

.btn-hover:hover {
  transform: scale(1.03);
}

@media (max-width:768px) {
  .reverse {
    flex-direction: column-reverse;
  }

  .md-none {
    display: none;
  }

  .mini-title-sec {
    text-align: center !important;
  }

  .mini-title-sec p {
    text-align: center !important;
    margin-bottom: 20px;
  }
}
</style>