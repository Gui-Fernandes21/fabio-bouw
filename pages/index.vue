<script setup lang="ts">
import { onMounted } from 'vue';

const isMobile = useState('mobile-view', () => false);

onMounted(() => {
  isMobile.value = window.innerWidth < 768;
  window.addEventListener('resize', () => {
    isMobile.value = window.innerWidth < 768;
  });
});
</script>

<template>
	<TheNav></TheNav>
  
  <MobilePage v-if="isMobile"/>
  <DesktopPage v-else />

  <TheFooter></TheFooter>
</template>

<style scoped></style>
 