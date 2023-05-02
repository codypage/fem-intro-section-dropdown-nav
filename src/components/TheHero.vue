<template>
  <section class="hero">
    <div class="hero__content">
      <h1 class="hero__title">
        Make <br />
        remote work
      </h1>
      <p class="hero__subtitle">
        Get your team in sync, no matter your location. Streamline processes, create team rituals,
        and watch productivity soar.
      </p>
      <a href="#" class="hero__button"> Learn more </a>
    </div>
    <div class="hero__image">
      <img src="../assets/images/image-hero-mobile.png" alt="" />
    </div>
  </section>
</template>

<style scoped lang="scss">
@media (min-width: 376px) {
  .hero__image > img {
    content: url(../assets/images/image-hero-desktop.png);
  }
}

.hero {
  margin-inline: auto;
  display: grid;
  grid-template-columns: 1fr 1fr;
  place-items: center;

  &__content {
    max-width: 540px;
    grid-column: 1/2;
  }

  &__image {
    grid-column: 2/2;
    margin-left: 125px;
  }
}
</style>
