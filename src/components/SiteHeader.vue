<script setup>
import { ref } from 'vue'

const menuOpen = ref(false)
const toggleMenu = () => { menuOpen.value = !menuOpen.value }
const closeMenu = () => { menuOpen.value = false }
</script>

<template>
  <header class="wrap nav">
    <a class="brand" href="#home" aria-label="禾院小馆首页"><span class="brand-mark">禾</span><span class="brand-name">禾院小馆<span class="brand-sub">HE YUAN · SEASONAL KITCHEN</span></span></a>
    <nav class="nav-links" :class="{ open: menuOpen }"><a href="#menu" @click="closeMenu">时令菜单</a><a href="#story" @click="closeMenu">关于禾院</a><a href="#visit" @click="closeMenu">来店坐坐</a></nav>
    <a class="nav-cta" href="#visit">预约一席 <span>↗</span></a>
    <button class="menu-toggle" aria-label="打开导航" :aria-expanded="menuOpen" @click="toggleMenu">{{ menuOpen ? '×' : '☰' }}</button>
  </header>
</template>
