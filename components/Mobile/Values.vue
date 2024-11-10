<template>
  <section class="values">
    <header>
      <h1>Nos Valeurs</h1>
    </header>

    <div class="container">

      <div class="card-container">
        <!-- <img src="/svg/vertical-lines.svg" class="vertical-line" alt="vertical lines" /> -->
        <div class="card">
          <img src="/images/quality-picture.png" class="pic" alt="quality picture" />
          <h3 class="title">Qualité</h3>
          <p class="description">Nous utilisons uniquement des matériaux de haute qualité et des techniques éprouvées pour garantir la durabilité et la solidité de nos réalisations.</p>
        </div>
        <!-- <img src="/svg/vertical-lines.svg" class="vertical-line" alt="vertical lines" /> -->
        <div class="card">
          <img src="/images/reliability-picture.png" class="pic" alt="reliability picture" />
          <h3 class="title">Fiabilité</h3>
          <p class="description">Nous nous engageons à respecter les délais et à honorer nos engagements envers nos clients.</p>
        </div>
        <!-- <img src="/svg/vertical-lines.svg" class="vertical-line" alt="vertical lines" /> -->
        <div class="card">
          <img src="/images/professional-picture.png" class="pic" alt="professional picture" />
          <h3 class="title">Professionnalisme</h3>
          <p class="description">Notre équipe travaille avec intégrité, transparence, et un service client irréprochable.</p>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.vertical-line {
  position: absolute;
  left: 40%;
  top: -2.5rem;
  z-index: 1;
  transform: none;
}

.card-container {
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 2.8rem 1rem;
  gap: 10px;
}

.card {
  position: relative;
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 10px;

  padding: 1rem;

  height: 100%;
  background: #fdfdfdc5;
  border-radius: 10px;

  transition: transform 200ms ease-in-out;

  & > h3 {
    font-family: 'DM Serif Display', sans-serif;
    font-size: var(--fb-header-3);
  }

  & > .pic {
    width: 90%;
    margin: 0 auto;
  }

  &:hover {
    transform: scale(1.02);
  }
}
</style>
