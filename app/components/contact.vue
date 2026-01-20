<template>
  <div class="contact">
    <div class="containr">
      <div class="row justify-content-center">
        <div class="col-lg-5 col-md-6 col-sm-12">
          <div class="form">
            <form class="bg-white p-4 rounded-4 shadow-sm" dir="rtl">
              <!-- الاسم + الهاتف -->
              <div class="row g-3 mb-3">
                <div class="col-12">
                  <label class="form-label">
                    الاسم الكامل <span class="text-danger">*</span>
                  </label>
                  <input
                    type="text"
                    class="form-control rounded-pill"
                    placeholder="أدخل اسمك الكامل"
                  />
                </div>
              </div>

              <!-- البريد + التاريخ -->
              <div class="row g-3 mb-3">
                <div class="col-md-6">
                  <label class="form-label">
                    رقم الهاتف <span class="text-danger">*</span>
                  </label>
                  <input
                    type="tel"
                    class="form-control rounded-pill"
                    placeholder="أدخل رقم الهاتف للتواصل"
                  />
                </div>
                <div class="col-md-6">
                  <label class="form-label">البريد الإلكتروني</label>
                  <input
                    type="email"
                    class="form-control rounded-pill"
                    placeholder="أدخل بريدك الإلكتروني"
                  />
                </div>
              </div>

              <!-- نوع الفعالية -->
              <div class="mb-3">
                <label class="form-label">نوع الفعالية</label>
                <select class="form-select rounded-pill">
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
                <textarea
                  class="form-control rounded-4"
                  rows="4"
                  placeholder="اكتب تفاصيل طلبك أو استفسارك"
                ></textarea>
                <small class="text-muted"> يرجى إدخال الأحرف على الأقل </small>
              </div>

              <!-- زر الإرسال -->
              <div class="text-center">
                <button
                  type="submit"
                  class="btn btn-lg w-100 text-white rounded-pill"
                  style="background: linear-gradient(90deg, #7f1469, #4b1366)"
                >
                 سجلي الأن
                </button>
              </div>
            </form>
          </div>
        </div>
        <div class="col-lg-5 col-md-6 col-sm-12"></div>
      </div>
    </div>
  </div>
</template>
