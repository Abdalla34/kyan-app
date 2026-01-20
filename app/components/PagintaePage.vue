<template>
    <div class="transitions-pages">
      <div class="parent p-3">
        <div class="container text-end">
          <NuxtLink to="/" class="fw-bold title-home text-black">الرئيسية</NuxtLink>
          <span class="fw-bold"> > </span>
          <span class="fw-bold">{{ pageTitle }}</span>
        </div>
      </div>
    </div>
  </template>
  
  <script setup>
  const route = useRoute();
  const pageTitle = computed(() => {
    return route.meta.title || route.name;
  });
  </script>
  
  <style scoped>
  .parent {
    background-color: rgb(243 245 247 / 1);
  }
  .title-home{
    text-decoration: none;
  }
  .title-home:hover {
    cursor:pointer;
    color: var(--second-color-bg) !important;
  }
  </style>