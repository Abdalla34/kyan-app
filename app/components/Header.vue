<template>
    <div class="header p-3" :class="{
        'bg-white': scrolled,
        'top': scrolled,
    }">
        <div class="container">
            <div class="row justify-content-between align-items-center ">
                <div class="col-lg-3 hide-media">
                    <div class="links-icon d-flex align-items-center justify-content-center gap-2">
                        <div class="mb-3 mb-md-0">
                            <a href="#" class="social-icon"><i class="bi bi-telephone"></i></a>
                            <a href="#" class="social-icon"><i class="bi bi-whatsapp"></i></a>
                            <a href="#" class="social-icon"><i class="bi bi-facebook"></i></a>
                            <a href="#" class="social-icon"><i class="bi bi-instagram"></i></a>
                        </div>
                    </div>
                </div>
                <div class="col-lg-6 hide-media">
                    <div class="nav d-flex align-items-center justify-content-center">
                        <ul class="ul-nav d-flex align-items-center flex-row-reverse gap-3 justify-content-center">
                            <li>
                                <NuxtLink to="/" exact-active-class="active">الرئيسية</NuxtLink>
                            </li>
                            <li>
                                <NuxtLink to="/about" exact-active-class="active">عن كيان</NuxtLink>
                            </li>
                            <li>
                                <NuxtLink to="/services" exact-active-class="active">أركان المركز</NuxtLink>
                            </li>
                            <li>
                                <NuxtLink to="/gallery" exact-active-class="active">معرض الصور</NuxtLink>
                            </li>
                            <li>
                                <NuxtLink to="/news" exact-active-class="active">جديدنا</NuxtLink>
                            </li>
                            <li>
                                <NuxtLink to="/blogs" exact-active-class="active">المدونة</NuxtLink>
                            </li>
                            <li>
                                <NuxtLink to="/contact" exact-active-class="active">تواصل معنا</NuxtLink>
                            </li>
                        </ul>
                    </div>
                </div>
                <div class="col-lg-3 media-mobile colp-sm-12 d-flex align-items-center justify-content-center">
                    <div class="image-head">
                        <img src="/logo.png" alt="">
                    </div>
                    <MobileMenu />
                </div>
            </div>
        </div>
    </div>
</template>
<script setup>
const showHeader = ref(true);
const scrolled = ref(false);
let lastScrollY = 0;

const handleScroll = () => {
    const currentScrollY = window.scrollY;

    if (currentScrollY > lastScrollY && currentScrollY > 100) {
        showHeader.value = false;
    } else {
        showHeader.value = true;
    }

    scrolled.value = currentScrollY > 0;

    lastScrollY = currentScrollY;
};

onMounted(() => {
    lastScrollY = window.scrollY;
    scrolled.value = window.scrollY > 0;
    window.addEventListener("scroll", handleScroll);
});

onBeforeUnmount(() => {
    window.removeEventListener("scroll", handleScroll);
});
</script>
<style scoped>
.header {
    position: fixed;
    top: 30px;
    left: 0;
    width: 100%;
    z-index: 10;
}

.top {
    top: 0;
    box-shadow: 0px 10px 30px rgb(0,0,0, 0.1);
}

a {
    text-decoration: none;
    color: rgb(17 24 39 / var(--tw-text-opacity, 1));
    font-weight: bold;
    font-size: 16px;
}

a:hover {
    color: rgb(26 174 230 / 1);
}
.active{
    color: rgb(26 174 230 / 1); 
    font-weight: bold;
}

@media (max-width:768px) {
    .hide-media {
        display: none;
    }

    .image-head img {
        width: 120px;
    }

    .media-mobile {
        justify-content: space-between !important;
    }
    .header {
    top: 0 !important;
    box-shadow: 0px 10px 30px rgb(0,0,0, 0.1);
}
}
</style>