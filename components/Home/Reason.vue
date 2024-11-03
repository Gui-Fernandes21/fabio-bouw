<template>
  <section class="reason">
    <div class="container">
      <header>
        <h2>Pourquoi Choisir</h2>
        <h1>Fabio Bouw</h1>
        <span>?</span>
      </header>
      <p>
        En choisissant nous, vous optez pour un partenaire de confiance pour vos projets de construction. Nous mettons un point 
        d’honneur à offrir des solutions personnalisées, adaptées à chaque projet, avec une attention particulière aux détails et
        aux finitions.
      </p>
    </div>
  </section>
</template>

<style scoped>
.container {
  margin: 2rem auto;
  width: 50%;
  text-align: center;
}

section {
  margin: 8rem 2rem;
}

  p {
    width: 80%;
    margin: 0 auto;
    font-weight: 200;
  }

header {
  position: relative;
  margin: 0 auto;
  width: max-content;

  display: flex;
  flex-direction: column;

  font-family: "DM Serif Display", sans-serif;

  h1 {
    border: none;
  }

  span {
    position: absolute;
    font-size: 4rem;
    color: var(--fb-primary);

    right: 0;
    bottom: 1.4rem;
  }
}
</style>
