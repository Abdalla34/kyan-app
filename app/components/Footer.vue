<template>
  <footer class="bg-light pt-5">
    <div class="container">
      <div class="row text-end">
        <!-- تابع يوميات طفلك -->
        <div class="col-lg-4 col-md-6 mb-4">
          <h5 class="fw-bold text-primary mb-3">تابع يوميات طفلك الصغير</h5>
          <p class="text-muted">
            تفاعل مع أنشطة طفلك، اطلع على صور وتقارير يومية، ومتابعة فورية
            ليومياته والأنشطة داخل الحضانة.
          </p>

          <div class="d-flex justify-content-end gap-2">
            <img
              src="https://developer.apple.com/assets/elements/badges/download-on-the-app-store.svg"
              alt="App Store"
              height="40"
            />
            <img
              src="https://upload.wikimedia.org/wikipedia/commons/7/78/Google_Play_Store_badge_EN.svg"
              alt="Google Play"
              height="40"
            />
          </div>
        </div>

        <!-- روابط سريعة -->
        <div class="col-lg-2 col-md-6 mb-4">
          <h5 class="fw-bold text-primary mb-3">روابط سريعة</h5>
          <ul class="list-unstyled">
            <li class="mb-2"><a href="#" class="footer-link">عن كيان</a></li>
            <li class="mb-2"><a href="#" class="footer-link">معرض الصور</a></li>
            <li class="mb-2"><a href="#" class="footer-link">تواصل معنا</a></li>
            <li class="mb-2"><a href="#" class="footer-link">جديدنا</a></li>
            <li class="mb-2"><a href="#" class="footer-link">المدونة</a></li>
          </ul>
        </div>

        <!-- مركز كيان المستقبل -->
        <div class="col-lg-4 col-md-6 mb-4">
          <h5 class="fw-bold text-primary mb-3">مركز كيان المستقبل</h5>
          <p class="text-muted">
            مركز كيان المستقبل لرعاية الأطفال، بيئة تعليمية آمنة تساعد على تنمية
            مهارات الطفل وبناء شخصيته في جو مليء بالحب والرعاية.
          </p>
        </div>

        <!-- اللوجو -->
        <div class="col-lg-2 col-md-6 mb-4 text-center text-lg-end">
          <img
            src="/logo.png"
            alt="logo"
            class="img-fluid mb-2"
            style="max-width: 120px"
          />
          <p class="fw-bold text-primary mb-0">مركز كيان المستقبل</p>
          <small class="text-muted">تنمية الأطفال</small>
        </div>
      </div>

      <hr />

      <!-- Bottom -->
      <div
        class="d-flex flex-column flex-md-row justify-content-between align-items-center pb-3"
      >
        <!-- Social -->
        <div class="mb-3 mb-md-0">
          <a href="#" class="social-icon"><i class="bi bi-telephone"></i></a>
          <a href="#" class="social-icon"><i class="bi bi-whatsapp"></i></a>
          <a href="#" class="social-icon"><i class="bi bi-facebook"></i></a>
          <a href="#" class="social-icon"><i class="bi bi-instagram"></i></a>
        </div>

        <!-- Copy -->
        <p class="mb-0 text-muted">
          © 2025 مركز كيان المستقبل - جميع الحقوق محفوظة
        </p>
      </div>
    </div>
  </footer>
</template>
<style scoped>
footer {
  direction: ltr;
}

.footer-link {
  color: #555;
  text-decoration: none;
}

.footer-link:hover {
  color: #0d6efd;
}

.social-icon {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  width: 36px;
  height: 36px;
  background: #eaf6ff;
  color: #0d6efd;
  border-radius: 50%;
  margin-left: 8px;
  text-decoration: none;
  font-size: 18px;
}

.social-icon:hover {
  background: #0d6efd;
  color: #fff;
}
</style>
