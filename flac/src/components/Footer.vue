<template>
  <footer className="footer">
    <div className="footer__content">
      <p className="footer__text">© 2024 Your Company. All rights reserved.</p>
      <nav className="footer__nav">
        <ul className="footer__nav-list">
          <li className="footer__nav-item">
            <a href="#" className="footer__nav-link">Privacy Policy</a>
          </li>
          <li className="footer__nav-item">
            <a href="#" className="footer__nav-link">Terms of Service</a>
          </li>
          <li className="footer__nav-item">
            <a href="#" className="footer__nav-link">Contact</a>
          </li>
        </ul>
      </nav>
    </div>
  </footer>
</template>

<script>
export default {
  name: 'FooterComponent',
};
</script>

<style scoped>
.footer {
  padding: 20px;
  background-color: #333;
  color: #fff;
  text-align: center;
}

.footer__content {
  max-width: 1200px;
  margin: 0 auto;
}

.footer__nav {
  margin-top: 10px;
}

.footer__nav-list {
  display: flex;
  justify-content: center;
  list-style: none;
  margin: 0;
  padding: 0;
}

.footer__nav-item {
  margin-right: 20px;
}

.footer__nav-link {
  color: #fff;
  text-decoration: none;
}

.footer__nav-link:hover {
  text-decoration: underline;
}
</style>
