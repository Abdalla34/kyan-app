<template>
    <div>
      <!-- Burger Button -->
      <button class="burger-btn" @click="toggleMenu">
        &#9776;
        <!-- أيقونة البرجر -->
      </button>
      <div 
        v-if="isOpen" 
        class="overlay" 
        @click="closeMenu"
      ></div>
  
      <!-- Mobile Menu -->
      <div class="mobile-menu p-2" :class="{ open: isOpen }">
        <div class="d-flex align-items-start justify-content-between mb-5">
          <div class="logo">
            <img src="/logo.png" alt="" style="width: 80px" />
          </div>
          <div @click="closeMenu" class="btn-close">
            <button class="close-btn" @click="closeMenu"></button>
          </div>
        </div>
        <ul class="text-end">
          <li class="link">
            <nuxt-link
              to="/"
              active-class="active"
              class="text-black a fs-6 fw-bold text-capitalize"
              @click="closeMenu"
            >
              الرئيسية</nuxt-link
            >
          </li>
          <li class="link">
            <nuxt-link
              to="/about"
              active-class="active"
              class="text-black a fs-6 fw-bold text-capitalize"
              @click="closeMenu"
            >
              من نحن</nuxt-link
            >
          </li>
          <li class="link">
            <nuxt-link
              @click="closeMenu"
              to="/our-services"
              active-class="active"
              class="text-black a fs-6 fw-bold text-capitalize"
            >
              خدماتنا</nuxt-link
            >
          </li>
          <li class="link">
            <nuxt-link
              @click="closeMenu"
              to="/our-projects"
              active-class="active"
              class="text-black a fs-6 fw-bold text-capitalize"
            >
              مشاريعنا</nuxt-link
            >
          </li>
          <li class="link">
            <nuxt-link
              @click="closeMenu"
              to="/blog"
              active-class="active"
              class="text-black a fs-6 fw-bold text-capitalize"
            >
              المدونه</nuxt-link
            >
          </li>
          <li class="link">
            <nuxt-link
              @click="closeMenu"
              to="/contact-us"
              active-class="active"
              class="text-black a fs-6 fw-bold text-capitalize"
            >
              للتواصل معنا</nuxt-link
            >
          </li>
        </ul>
      </div>
    </div>
  </template>
  
  <script setup>
  const isOpen = ref(false);
  function toggleMenu() {
    isOpen.value = !isOpen.value;
  }
  
  function closeMenu() {
    isOpen.value = false;
  }
  </script>
  
  <style scoped>
  /* Burger button */
  .burger-btn {
    display: none;
    font-size: 20px;
    background: none;
    border: none;
    cursor: pointer;
    position: fixed;
    top: 1rem;
    right: 1rem;
    z-index: 99;
    width: 40px;
    height: 40px;
    background-color: #f3f4f6;
    border-radius: 50%;
  }
  .overlay {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-color: rgba(0,0,0,0.5); /* نص شفاف أسود */
    z-index: 50; /* تحت المينيو */
  }
  
  /* Mobile menu */
  .mobile-menu {
    display: none;
    background-color: #fff;
    border-left: 1px solid #ccc;
    position: fixed;
    top: 0;
    right: -100%;
    width: 80%;
    height: 100%;
    z-index: 100;
    transition: right 0.3s ease;
  }
  
  .mobile-menu.open {
    right: 0;
  }
  
  ul li:first-child {
    border-bottom: 2px solid black;
    padding: 10px;
  }
  ul li {
    border-bottom: 1px solid #e5e7eb;
    padding: 10px;
  }
  .a {
    text-align: end;
  }
  .close-btn {
    font-size: 2rem;
    background: none; /* مفيش لون خلفية */
    border: none;
    cursor: pointer;
    position: absolute;
    top: 1rem;
    right: 1rem;
  }
  
  /* Show burger and menu only on mobile */
  @media (max-width: 768px) {
    .burger-btn {
      display: block;
    }
  
    .mobile-menu {
      display: block;
    }
  }
  </style>