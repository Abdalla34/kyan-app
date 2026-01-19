<template>
    <div class="header p-3" :class="{
        'bg-white': scrolled,
    }">
        <div class="container">
            <div class="row justify-content-between align-items-center ">
                <div class="col-lg-3 hide-media">
                    <div class="links-icon d-flex align-items-center justify-content-center gap-2">
                        <div class="face">test</div>
                        <div class="whats">test</div>
                        <div class="instgram">test</div>
                        <div class="snap">test</div>
                        <div class="call">test</div>
                    </div>
                </div>
                <div class="col-lg-6 hide-media">
                    <div class="nav d-flex align-items-center justify-content-center">
                        <ul class="ul-nav d-flex align-items-center flex-row-reverse gap-3 justify-content-center">
                            <li>
                                <NuxtLink to="/">الرئيسية</NuxtLink>
                            </li>
                            <li>
                                <NuxtLink to="/about">عن كيان</NuxtLink>
                            </li>
                            <li>
                                <NuxtLink to="/center-pillars">أركان المركز</NuxtLink>
                            </li>
                            <li>
                                <NuxtLink to="/galley">معرض الصور</NuxtLink>
                            </li>
                            <li>
                                <NuxtLink to="/news">جديدنا</NuxtLink>
                            </li>
                            <li>
                                <NuxtLink to="/blogs">المدونة</NuxtLink>
                            </li>
                            <li>
                                <NuxtLink to="/contact">تواصل معنا</NuxtLink>
                            </li>
                        </ul>
                    </div>
                </div>
                <div class="col-lg-3 d-flex align-items-center justify-content-center">
                    <div class="image-head">
                        <img src="/logo.png" alt="">
                    </div>
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
    top: 0;
    left: 0;
    width: 100%;
    z-index: 10;
    /* box-shadow: 0px 5px 90px rgba(0, 0, 0, 0.1); */
}


a {
    text-decoration: none;
    color: rgb(17 24 39 / var(--tw-text-opacity, 1));
    font-weight: 800;
    font-size: 16px;
}

@media (max-width:768px) {

    .hide-media {
        display: none;
    }

    .image-head img {
        width: 100px;
    }
}
</style>