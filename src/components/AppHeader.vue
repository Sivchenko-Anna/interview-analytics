<script setup lang="ts">
import { ref } from 'vue'
import AppMenubar from '@/main'

const menuItems = ref([
  {
    label: 'Авторизация',
    icon: 'pi pi-user',
    path: '/auth'
  },
  {
    label: 'Добавить',
    icon: 'pi pi-plus',
    path: '/'
  },
  {
    label: 'Список собеседований',
    icon: 'pi pi-list',
    path: '/list'
  },
  {
    label: 'Статистика',
    icon: 'pi pi-chart-pie',
    path: '/statistic'
  }
])
</script>

<template>
  <app-menubar :model="menuItems" class="menu" />
</template>

<style scoped>
  .menu {
    margin: 30px 0;
  }

  .menu-exit {
    cursor: pointer;
  }
</style>
