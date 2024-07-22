<template>
  <header class="header">
    <div class="header__container">
      <a href="#" class="header__logo">
        <img src="@/assets/img/header/logo.png" alt="Logo">
      </a>
      <div class="header__nav">
        <div class="header__nav-list">
          <div class="header__nav-item">
            <li><a href="#">Features</a></li>
          </div>
          <div class="header__nav-item">
            <li><a href="#">Developers</a></li>
          </div>
          <div class="header__nav-item">
            <li><a href="#">Company</a></li>
          </div>
          <div class="header__nav-item">
            <li><a href="#">Blog</a></li>
          </div>
          <div class="header__nav-item">
            <li><a href="#">Changelog</a></li>
          </div>
        </div>
      </div>
      <div class="header__cta">
        <button class="header__cta-button">Join waitlist</button>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  name: 'HeaderComponent',
};
</script>

<style scoped>
.header {
  padding: 13px 191px;
  width: auto;
  background-color: #020103;
  font-size: 13px;
  line-height: 26px;
  color: rgba(255, 255, 255, 0.6);
  text-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
}
.header__container {
  display: flex;
  flex-direction: row;
  align-items: center;
  gap: 74px;
  width: fit-content;
  margin: 0 auto;
}
.header__logo {
  width: 38px;
  height: 38px;
}
.header__nav-list {
  display: flex;
  flex-direction: row;
  align-items: center;
  gap: 30px;
  padding: 8px 40px;
  border: 1px solid rgba(255, 255, 255, 0.15);
  border-radius: 60px;
}
.header__cta {
  padding: 6px;
  width: 121px;
  height: 42px;
  border: 1px solid rgba(255, 255, 255, 0.15);
  border-radius: 12px;
}
.header__cta-button {
  width: 109px;
  height: 30px;
  background: rgba(140, 69, 255, 0.4);
  border: 1px solid rgba(255, 255, 255, 0.15);
  box-shadow: inset 0px 0px 6px 3px rgba(255, 255, 255, 0.25);
  backdrop-filter: blur(7px);
  /* Note: backdrop-filter has minimal browser support */
  border-radius: 8px;
  color: #FFFFFF;
  cursor: pointer;
}
</style>
