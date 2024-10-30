<template>
  <section class="footer">
    <img src="/images/fabio-bouw-white.png" alt="FB logo" />
    <p>© 2024 Fabio Bouw. All Rights Reserved</p>
    <span>Designed & Developed by <a href="www.gui-fernandes.com" target="_blank">Gui Fernandes</a></span>
  </section>
</template>

<style scoped>
section {
  width: 100%;
  height: 12rem;
  background: var(--fb-primary);

  margin-bottom: 0;

  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;

  & > span {
    font-family: 'DM Sans', sans-serif;
    font-size: var(--fb-span);
    margin: 3px 0;

    & > a {
      color: white;
    }
  }
}
img {
  filter: brightness(1000%);
  height: 6rem;
}
</style>