<template>
  <div class="hello">
    <header>
      <nav class="navbar">
        <ul>
          <li>
            <a class="link" href="">Gmail</a>
          </li>
          <li>
            <a class="link" href="">Imagini</a>
          </li>
          <li>
            <a href=""><fa class="menu-icon" icon="bars"></fa></a>
          </li>
          <li>
            <button>Sign In</button>
          </li>
        </ul>
      </nav>
    </header>

    <section class="content-section">
      <div class="content-wrapper">
        <img class="logo-img" src="@/assets/logo.jpg" alt="Google Logo" />
        <div class="search-bar">
          <fa icon="search"></fa>
          <input class="search-input" type="text">
          <fa icon="keyboard"></fa>
          <fa icon="microphone"></fa>
        </div>
      </div>
      <div class="search-btns">
        <button class="google-search-btn">Căutare Google</button>
        <button class="lucky-search-btn">Mă simt norocos</button>
      </div>
      <div class="languages">
        <p>
          Google oferit în: 
          <a href="">English</a>
          <a href="">Magyar</a>
          <a href="">Deutsch</a>
        </p>
      </div>
    </section>

    <footer>
      <div class="footer-content upper-footer">
        <p>România</p>
      </div>
      <div class="footer-content lower-footer">
        <ul class="lower-left-footer">
          <li>
            <a href="">Despre</a>
          </li>
          <li>
            <a href="">Publicitate</a>
          </li>
          <li>
            <a href="">Companii</a>
          </li>
          <li>
            <a href="">Cum funcționează căutarea</a>
          </li>
        </ul>
        <ul class="lower-right-footer">
          <li>
            <a href="">Confidențialitate</a>
          </li>
          <li>
            <a href="">Termeni</a>
          </li>
          <li>
            <a href="">Setări</a>
          </li>
        </ul>
      </div>
    </footer>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped></style>
