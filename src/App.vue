<script setup lang="ts">
import AppProvider from '@/components/AppProvider.vue'
</script>

<template>
  <AppProvider>
    <router-view v-slot="{ Component }">
      <component :is="Component" />
    </router-view>
  </AppProvider>
</template>
