<template>
  <header class="header">
    <div class="header__logo">
<!--      <img src="path-to-logo.png" alt="Logo" />-->
    </div>
    <nav class="header__nav">
      <ul class="header__nav-list">
        <li class="header__nav-item">
          <a href="#" class="header__nav-link">Home</a>
        </li>
        <li class="header__nav-item">
          <a href="#" class="header__nav-link">About</a>
        </li>
        <li class="header__nav-item">
          <a href="#" class="header__nav-link">Contact</a>
        </li>
      </ul>
    </nav>
  </header>
</template>

<script>
export default {
  name: 'HeaderComponent',
};
</script>

<style scoped>
.header {
  display: flex;
  justify-content: space-between;
  padding: 20px;
  background-color: #333;
  color: #fff;
}

.header__logo img {
  height: 40px;
}

.header__nav {
  display: flex;
  align-items: center;
}

.header__nav-list {
  display: flex;
  list-style: none;
  margin: 0;
  padding: 0;
}

.header__nav-item {
  margin-right: 20px;
}

.header__nav-link {
  color: #fff;
  text-decoration: none;
}

.header__nav-link:hover {
  text-decoration: underline;
}
</style>
