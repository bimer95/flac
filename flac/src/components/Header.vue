<template>
  <header class="header">
    <div class="header__container">
      <a href="#" class="header__logo">
        <img src="@/assets/img/header/logo.png" alt="Logo">
      </a>
      <nav class="header__nav">
          <ul class="header__nav-list">
            <li class="header__nav-item" >
              <Dropdown title="Features" v-bind:items="features" />
            </li>
            <li class="header__nav-item" >
              <a class="header__nav-link" href="#">Developers</a>
            </li>
            <li class="header__nav-item" >
              <Dropdown title="Company" v-bind:items="company" />
            </li>
            <li class="header__nav-item" >
              <a class="header__nav-link" href="#">Blog</a>
            </li>
            <li class="header__nav-item" >
              <a class="header__nav-link" href="#">Changelog</a>
            </li>
          </ul>
      </nav>
      <div class="header__cta">
        <button class="header__cta-button">Join waitlist</button>
      </div>
    </div>
  </header>
</template>

<script>
import Dropdown from "@/components/ui/Dropdown.vue";
export default {
  name: 'HeaderComponent',
  components: {Dropdown},
  data() {
    return {
      features: [
        { title: "Integration", link: "#" },
        { title: "Updates", link: "#" },
        { title: "Security", link: "#" },
        { title: "Docs", link: "#" },
        { title: "Pricing", link: "#" }
      ],
      company: [
        { title: "About", link: "#" },
        { title: "Careers", link: "#" },
        { title: "Press", link: "#" },
        { title: "Manifesto", link: "#" }
      ]
    }
  }
};
</script>

<style scoped>
.header {
  padding: 13px 0;
  width: auto;
  background-color: #020103;
  font-size: 13px;
  line-height: 26px;
  color: #FFFFFF99;
  text-shadow: 0 4px 4px rgba(0, 0, 0, 0.25);
}
.header__container {
  max-width: 1200px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  gap: 74px;
  margin: 0 auto;
}
.header__logo {
  width: 38px;
  height: 38px;
}
.header__nav-list {
  display: flex;
  align-items: center;
  gap: 30px;
  padding: 5px 40px;
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
  box-shadow: inset 0 0 6px 3px rgba(255, 255, 255, 0.25);
  backdrop-filter: blur(7px);
  /* Note: backdrop-filter has minimal browser support */
  border-radius: 8px;
  color: #FFFFFF;
  cursor: pointer;
}

</style>
