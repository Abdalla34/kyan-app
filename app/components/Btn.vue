<template>
    <div class="btn">
        <button class="btn-main text-white rounded-5 px-4 py-2">
            {{ text }}
        </button>
    </div>
</template>
<script setup>
defineProps({
    text: String
})
</script>
<style scoped>
.btn-main {
    outline: none;
    border: none;
    background: linear-gradient(to right, #1aaee6, #0d607f);
    transition: all 0.2s ease-in-out;
}
.btn-main:hover {
transform: scale(1.03);
box-shadow: 0px 20px 50px rgb(0, 0, 0 , 0.2) ;
}
</style>