<template>
  <section class="values">
    <header>
      <h1>Nos Valeurs</h1>
    </header>

    <div class="container">
      <img src="/svg/vertical-lines.svg" alt="vertical lines" />

      <div class="card-container">
        <div class="card">
          <img src="/images/quality-picture.png" alt="quality picture" />
          <h2 class="title">Qualité</h2>
          <p class="description">Nous utilisons uniquement des matériaux de haute qualité et des techniques éprouvées pour garantir la durabilité et la solidité de nos réalisations.</p>
        </div>
        <div class="card">
          <img src="/images/reliability-picture.png" alt="reliability picture" />
          <h2 class="title">Fiabilité</h2>
          <p class="description">Nous nous engageons à respecter les délais et à honorer nos engagements envers nos clients.</p>
        </div>
        <div class="card">
          <img src="/images/professional-picture.png" alt="professional picture" />
          <h2 class="title">Professionnalisme</h2>
          <p class="description">Notre équipe travaille avec intégrité, transparence, et un service client irréprochable.</p>
        </div>
      </div>
      <img src="/svg/horizontal-lines.svg" class="horizontal" alt="horizontal line">

      <img src="/svg/vertical-lines.svg" alt="vertical lines" />
    </div>
  </section>
</template>

<style scoped>
.container {
  display: flex;
  position: relative;
}
.horizontal {
  position: absolute;
  z-index: 0;
  top: 40%;
}


.card-container {
  display: flex;
  align-items: center;
  padding: 2.8rem 1rem;
  gap: 10px;
  z-index: 10;
}

.card {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 10px;

  padding: 1rem;
  
  height: 100%;
  background: #fdfdfdc5;
  border-radius: 10px;

  transition: transform 200ms ease-in-out;

  & > h2 {
    font-family: 'DM Serif Display', sans-serif;
    font-size: var(--fb-header-3);
  }

  & > img {
    width: 90%;
    margin: 0 auto;
  }

  &:hover {
    transform: scale(1.02);
  }
}
</style>
