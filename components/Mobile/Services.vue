<template>
  <section class="services">
    <header>
      <h1>Nos Services</h1>
    </header>

    <div class="container">
      <div class="card">
        <img src="/images/ceiling-machine.png" alt="ceiling-machine" />
        <div class="content">
          <h3>Travaux de Gyproc</h3>
          <p>
            Chez Fabio Bouw, nous sommes spécialisés dans les travaux de gyproc, offrant des solutions d'aménagement intérieur sur mesure pour vos projets de construction et de rénovation. Que vous ayez besoin de cloisons, de plafonds suspendus ou
            d'isolation acoustique, notre équipe d'experts est dédiée à réaliser vos idées avec précision et professionnalisme.
          </p>
        </div>
      </div>
      <div class="card">
        <img src="/images/mdf-work.jpg" alt="mdf work" />
        <div class="content">
          <h3>Travaux de MDF</h3>
          <p>
            Chez Fabio Bouw, nous sommes spécialisés dans les travaux de MDF, offrant des solutions sur mesure pour tous vos projets d'aménagement intérieur. Que vous souhaitiez des meubles intégrés, des cloisons décoratives ou des finitions
            élégantes, notre équipe d'artisans qualifiés est dédiée à réaliser vos idées avec précision et esthétisme.
          </p>
        </div>
      </div>
      <div class="card">
        <img src="/images/mezzanine-work.jpg" alt="mezzanine work" />
        <div class="content">
          <h3>Travaux de Mezanine</h3>
          <p>
            Chez Fabio Bouw, nous sommes experts en conception et construction de mezzanines, offrant des solutions sur mesure pour optimiser l'espace de vos intérieurs résidentiels et commerciaux. Notre savoir-faire vous permet d'ajouter une
            dimension supplémentaire à votre espace, alliant fonctionnalité et esthétisme.
          </p>
        </div>
      </div>
      <div class="card">
        <img src="/images/osb-work.jpg" alt="osb work" />
        <div class="content">
          <h3>Travaux de OSB</h3>
          <p>
            Chez Fabio Bouw, nous sommes spécialisés dans les travaux d'OSB, offrant des solutions solides et durables pour tous vos projets de construction et de rénovation. Que ce soit pour des planchers, des murs, des toitures ou des cloisons,
            notre équipe d'experts s'engage à réaliser vos projets avec précision et professionnalisme.
          </p>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.container {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}
.card {
  width: 90%;
  height: 100%;
  margin: 2rem;
  padding: 1rem;

  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  gap: 10px;

  background: var(--fb-white);
  border-radius: 5px;

  & > img {
    width: 95%;
    height: 15rem;
    border-radius: 5px;
  }
}

.content {
  display: flex;
  flex-direction: column;
  gap: 5px;

  & > p {
    font-size: 14px;
  }

  & > h3 {
    font-size: var(--fb-header-3);
    font-family: 'DM Serif Display', sans-serif;
  }
}
</style>
