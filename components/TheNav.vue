<template>

  <nav>
    <div class="logo">
      <img src="/images/fabio-bouw-white.png" alt="Fabio Bouw Logo">
    </div>
  </nav>

</template>

<style scoped>
nav {
  background: var(--fb-primary);
  width: 100%;
  height: 6rem;
}
.logo {
  width: 100%;
  display: flex;
  justify-content: center;
  align-items: center;

  padding-top: .5rem;
}

.logo, img { 
  height: 100%;
  filter: brightness(1000%);
}
</style>