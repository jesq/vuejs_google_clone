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
            <div class="circle-shadow">
              <a href=""><fa class="menu-icon" icon="bars"></fa></a>
            </div>
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
<style scoped>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

li {
  list-style-type: none;
}

a {
  text-decoration: none;
}

body {
  font-family: sans-serif;
  height: 100vh;
  display: flex;
  flex-direction: column;
}

/* Header */

header {
  border: 1px solid red;
  height: 60px;
}

.navbar {
  height: 100%;
  width: 100%;
  padding: 10px 20px;
}

.navbar ul {
  height: 100%;
  display: flex;
  justify-content: flex-end;
  align-items: center;
  font-size: 14px;
}

.navbar ul li {
  margin-left: 15px;
}

.navbar ul li a {
  color: black;
}

.link:hover {
  text-decoration: underline;
}

.navbar button {
    border: 1px solid #4285f4;
    font-weight: bold;
    outline: none;
    background: #4285f4;
    color: #fff;
    padding: 5px 10px;
    border-radius: 3px;
    margin-left: 4px;
    cursor: pointer;
}

.circle-shadow {
  height: 40px;
  width: 40px;
  border-radius: 50%;
  display: flex;
  justify-content: center;
  align-items: center;
}

.circle-shadow:hover {
  background-color: rgba(0, 0, 0, 0.1);
}

</style>
