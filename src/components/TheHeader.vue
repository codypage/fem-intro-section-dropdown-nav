<template>
  <header>
    <nav class="nav">
      <div class="nav__logo">
        <a href="#">
          <img
            alt="Workit logo"
            class="logo"
            src="@/assets/images/logo.svg"
            width="87"
            height="35"
          />
        </a>
      </div>
      <ul class="nav__list">
        <li class="nav__item nav__item--dropdown">
          <a class="nav__link nav__link--dropdown" href="#"
            >Features <span class="nav__dropdown-icon"></span
          ></a>
          <ul class="nav__dropdown">
            <li class="nav__dropdown-item">
              <a class="nav__dropdown-link" href="#">Calendar</a>
            </li>
            <li class="nav__dropdown-item">
              <a class="nav__dropdown-link" href="#">Reminders</a>
            </li>
            <li class="nav__dropdown-item">
              <a class="nav__dropdown-link" href="#">Planning</a>
            </li>
          </ul>
        </li>
        <li class="nav__item nav__item--dropdown">
          <a class="nav__link nav__link--dropdown" href="#"
            >Company <span class="nav__dropdown-icon"></span
          ></a>
          <ul class="nav__dropdown">
            <li class="nav__dropdown-item">
              <a class="nav__dropdown-link" href="#">History</a>
            </li>
            <li class="nav__dropdown-item">
              <a class="nav__dropdown-link" href="#">Our Team</a>
            </li>
          </ul>
        </li>
        <li class="nav__item">
          <a class="nav__link" href="#">Careers</a>
        </li>
        <li class="nav__item">
          <a class="nav__link" href="#">About</a>
        </li>
      </ul>
      <div class="nav__buttons">
        <a class="nav__button" href="#">Log In</a>
        <a class="nav__button nav__button--primary" href="#">Register</a>
      </div>
    </nav>
  </header>
</template>

<style lang="scss">
@use '../assets/scss/utils' as *;

.nav {
  display: flex;
  justify-content: space-between;

  &__logo,
  &__list,
  &__buttons {
    display: flex;
    gap: 1rem;
    align-items: center;
    justify-content: center;
  }
}

.nav__button--primary {
  display: block;
  display: flex;
  align-items: center;
  justify-content: center;
  width: rem(104);
  height: rem(42);
  border: rem(1.5) solid #686868;
  border-radius: rem(14);
}

.nav__dropdown-item {
  display: none;
}

.nav__dropdown-icon {
  display: inline-block;
  width: rem(8);
  height: rem(4);
  margin-left: rem(9);
  background-image: url('../assets/images/icon-arrow-down.svg');
  background-position: center;
  transition: transform 0.2s;
}

.nav__dropdown-link:hover .nav__dropdown-icon:hover,
.nav__dropdown-link:focus .nav__dropdown-icon:focus {
  background-image: url('../assets/images/icon-arrow-up.svg');
}
</style>
