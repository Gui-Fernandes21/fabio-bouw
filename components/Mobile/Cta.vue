<script setup lang="ts">
import { useRouter } from 'vue-router';

const router = useRouter();

const contactPage = () => {
  router.push('/contact');
};
</script>

<template>
  <section class="cta">
    <img src="/svg/horizontal-lines.svg" alt="horizontal lines">
    <div class="cta-wrapper">
      <h1>Demande de devis gratuit</h1>
      <button class="btn" @click="contactPage">Contacter nous</button>
    </div>
  </section>

</template>

<style scoped>
section {
  position: relative;

  display: flex;
  justify-content: center;
  align-items: center;
}
img {
  position: absolute;
  z-index: 0;
  top: 40%;
}
.cta-wrapper {
  width: 90%;
  background-color: var(--fb-primary);
  border-radius: 10px;

  text-align: center;

  display: flex;
  flex-direction: column;
  justify-content: space-evenly;
  align-items: center;

  padding: 2rem;
  height: 20rem;

  z-index: 3;
}
h1 {
  color: var(--fb-offwhite);
}


</style>