<template>
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
    <section class="middle-section">
      <div class="content-wrapper">
        <img class="logo-img" src="@/assets/logo.jpg" alt="Google Logo"/>
        <div class="search-bar">
          <i><fa icon="search"></fa></i>
          <input class="search-input" type="text" />
          <i><fa icon="keyboard"></fa></i>
          <i><fa icon="microphone"></fa></i>
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
<style>
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

/* Header */

header {
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

/* Middle section */

.middle-section {
  flex-grow: 1;
  display: flex;
  justify-content: center;
  align-items: center;
  margin-top: 100px;
}

.content-wrapper {
  width: 100%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  padding:60px;
  padding-bottom:60px;
}

.logo-img {
  width: 300px;
  margin-bottom: 20px;
}

.search-bar {
  border:  1px solid lightgray;
  width: 600px;
  height: 45px;
  border-radius: 30px;
  display: flex;
  align-items: center;
  padding-left: 15px;
}

.search-bar:hover {
  border: 1px solid #fff;
    box-shadow: 0 0 2px rgba(0, 0, 0, 0.05),
                0 0 2px rgba(0, 0, 0, 0.05),
                0 0 3px rgba(0, 0, 0, 0.05),
                0 0 4px rgba(0, 0, 0, 0.05),
                0 0 5px rgba(0, 0, 0, 0.05),
                0 0 4px rgba(0, 0, 0, 0.05),
                0 0 5px rgba(0, 0, 0, 0.05)
}

.search-bar i {
  font-size: 18px;
  color: gray;
  margin-right: 15px;
  cursor: pointer;
}

.search-bar input {
  flex-grow: 1;
  height: 30px;
  margin-right: 15px;
  font-size: 16px;
  border: none;
}

.search-btns {
  margin-top: 20px;
}

.search-btns button {
  height: 40px;
  font-size: 14px;
  border: none;
  margin-left: 10px;
  color: black;
  background-color: #F2F3F4;
}

.search-btns button:hover {
  border: 1px solid lightgray;
}

.google-search-btn {
  width: 120px;
}

.lucky-search-btn {
  width: 140px;
}

.languages {
  margin-top: 20px;
  font-size: 14px;
}

.languages p a {
  color: blue;
  margin-left: 5px;
}

.languages p a:hover {
  text-decoration: underline;
}

/* Footer */

footer {
    background-color: #F2F2F2;
    height: 100px;
    position:absolute;
    bottom:0;
    width:100%;
}

.footer-content {
    display: flex;
    align-items: center;
    padding: 20px;
}

.upper-footer {
    height: 50%;
    border-bottom: 1px solid lightgray;
}

.upper-footer p {
    color: gray;
    font-size: 14px;
}

.lower-footer {
    height: 50%;
    display: flex;
    justify-content: space-between;
}

.lower-footer ul li a {
    font-size: 14px;
    color: gray;
}

.lower-footer ul li a:hover {
    text-decoration: underline;
}

.lower-left-footer {
    display: flex;
}

.lower-left-footer li {
    margin-right: 15px;
}


.lower-right-footer {
    display: flex;
}

.lower-right-footer li {
    margin-left: 15px;
}

@media only screen and (max-width: 650px) {
    /* Navbar */
    .navbar ul {
        font-size: 10px;
    }

    .menu-icon,
    .user-icon span {
        font-size: 14px;
    }

    .circle-shadow {
        height: 30px;
        width: 30px;
    }

    /* Logo */
    .logo-img {
        width: 200px;
    }

    /* Search Bar */
    .search-bar {
        width: 90%;
        height: 35px;
    }

    .search-bar i {
        font-size: 14px;
    }

    /* Buttons */
    .search-btns button {
        height: 30px;
        font-size: 12px;
    }

    .google-search-btn {
        width: 100px;
    }
    
    .lucky-search-btn {
        width: 120px;
    }

    /* Language */
    .languages {
        font-size: 12px;
    }

    /* Footer */
    footer {
        height: 150px;
    }

    .upper-footer {
        height: 50px;
    }

    .lower-footer {
        height: 100px;
        flex-direction: column;
    }

    .lower-left-footer {
        flex-wrap: wrap;
    }
}

</style>
