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
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
