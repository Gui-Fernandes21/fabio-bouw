<template>
  <section class="banner">
    <div class="img-section">
      <img src="/images/ceiling-machine.png" alt="ceiling machine" />
    </div>

    <div class="text-section">
      <p class="slogan">Solidité et précision, <br> Du toit aux murs.</p>
      <p class="expert">Experts en pose de Gyproc® <br> à Bruxelles et ses alentours</p>
    </div>
  </section>
</template>

<style scoped>
.banner {
  margin: 0;
  width: 100%;
  position: relative;
}
.img-section {
  display: flex;
  width: 100%;
  height: 50vh;
  overflow: hidden;
}

.text-section {
  position: absolute;
  bottom: -10rem;
  left: 2rem;
  height: 90%;
  width: 65%;
  background-color: var(--fb-primary);
  color: var(--fb-offwhite);
  border-radius: 10px;
  padding: 5rem 1rem;

  text-align: center;

  display: flex;
  flex-direction: column;
  justify-content: space-between;
  align-items: center;

  & > .slogan {
    font-size: var(--fb-header-4);
    font-weight: 300;
    line-height: 2.5rem;
  }

  & > .expert {
    font-size: var(--fb-header-4);
    font-weight: 100;
    line-height: 2.5rem;
  }

  & > h1 {
    font-size: var(--fb-header-1);
    border-bottom: 2px solid var(--fb-primary);
  }
}
</style>
