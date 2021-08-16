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
