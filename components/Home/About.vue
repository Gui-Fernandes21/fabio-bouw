<template>
  <img src="/svg/horizontal-lines.svg" alt="Horizontal lines" />
  <section class="about">
    <header>
      <h1>À propos de nous</h1>
    </header>
    <div class="grid">
      <p>
        Basée à Bruxelles, Fabio Bouw est une entreprise de construction spécialisée dans les travaux de gyproc, de toiture, et de cloisons sèches. Forts de plusieurs années d'expérience dans le secteur, nous nous engageons à fournir un service de
        qualité supérieure, fiable, et adapté aux besoins de nos clients.
        <br />
        <br />
        Notre équipe est composée de professionnels qualifiés qui partagent une passion pour l'excellence et un souci du détail. Chaque projet est pour nous une opportunité de démontrer notre expertise et notre engagement envers la satisfaction du
        client.
      </p>
      <img src="/images/fabio-bouw-black.png" alt="fabio bouw black logo" />
      <img src="/images/bxl-logo.png" alt="bxl logo" />
    </div>
  </section>
</template>

<style scoped>
.about {
  padding: 2rem;
}
header {
  /* width: 100%; */

  h1 {
    display: inline-block;
    font-size: var(--fb-header-1);
  }
}
.grid {
  display: grid;
  grid-template-columns: 2fr 1fr 1fr;
  place-items: center;
  padding: 1rem 0;

  & > img {
    height: 10rem;
    flex: 1;
  }
}
</style>
