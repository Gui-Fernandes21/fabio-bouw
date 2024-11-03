<template>

  <section class="cta">
    <img src="/svg/horizontal-lines.svg" alt="horizontal lines">
    <div class="cta-wrapper">
      <h1>Demande de devis gratuit</h1>
      <button>Contacter nous</button>
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
  width: 50%;
  background-color: var(--fb-primary);
  border-radius: 10px;

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
button {
  background: none;
  border: 2px solid var(--fb-offwhite);
  border-radius: 5px;
  cursor: pointer;
  color: var(--fb-offwhite);
  
  font-family: 'DM Sans', sans-serif;
  font-size: var(--fb-body);
  
  padding: 1rem 4rem;

  transition: all 150ms ease-in-out;

  &:hover {
    background: var(--fb-offwhite);
    color: var(--fb-primary);
  }
}

</style>