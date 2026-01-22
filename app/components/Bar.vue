<template>
    <div
      class="bottom-bar d-lg-none d-flex align-items-center justify-content-around"
      v-if="showBar"
    >
      <div class="icon-box" @click="navigateTo('/')">
        <IconsIconHome />
      </div>
  
      <div
        @click="navigateTo('/contact')"
        class="icon-box d-flex align-items-center justify-content-center"
      >
        <IconsIconDm />
      </div>
  
      <div class="icon-box" @click="navigateTo('/contact')">
        <IconsIconCall />
      </div>
  
      <div
        @click="scrollTop"
        class="icon-box arrow fs-5 fw-bold d-flex align-items-center justify-content-center"
      >
        ↑
      </div>
    </div>
  </template>
  
  <script setup>
  const showBar = ref(false);
  const router = useRouter();
  
  const handleScroll = () => {
    showBar.value = window.scrollY > 100; 
  };
  
  const scrollTop = () => {
    window.scrollTo({ top: 0, behavior: "smooth" });
  };
  
  const navigateTo = (path) => {
    router.push(path);
  };
  
  onMounted(() => {
    window.addEventListener("scroll", handleScroll);
  });
  
  onUnmounted(() => {
    window.removeEventListener("scroll", handleScroll);
  });
  </script>
  
  <style scoped>
  .bottom-bar {
    position: fixed;
    bottom: 0;
    left: 0;
    width: 100%;
    background-color: rgb(243 245 247 / 1);
    padding: 5px 0;
    box-shadow: 0 -2px 10px rgba(0, 0, 0, 0.2);
    transition: transform 0.3s ease, opacity 0.3s ease;
    z-index: 1000;
  }
  
  .icon-box {
    color: #4b5563;
    font-size: 17px;
    cursor: pointer;
    transition: transform 0.2s, background 0.2s;
    padding: 8px 12px;
    border-radius: 12px;
  }
  </style>