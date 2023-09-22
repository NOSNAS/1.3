<script setup>

</script>

<template>
  <div>
    <nav class="w3-sidebar w3-bar-block w3-small w3-hide-small w3-center">
      <!-- Router links for navigation -->
      <router-link to="/" class="sidebar-link">
        <i class="fa fa-home w3-xxlarge"></i>
        <p>HOME</p>
      </router-link>

      <router-link to="/about" class="sidebar-link">
        <i class="fa fa-user w3-xxlarge"></i>
        <p>ABOUT</p>
      </router-link>

      <router-link to="/contact" class="sidebar-link">
        <i class="fa fa-envelope w3-xxlarge"></i>
        <p>CONTACT</p>
      </router-link>
    </nav>
  </div>
  <footer>
    &copy; SIT 120 PORTFOLIO
  </footer>
  <RouterView />
</template>

<style scoped>

.title{
  font-family: Bradley Hand, cursive;
  color: azure;
  text-align: center;
  display: block;
  padding: 20px 25px;
}

nav {
  font-family: Monospace, serif;
}

ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  overflow: hidden;
  background-color: #333;
}

li {
  float: left;
}

li a {
  display: block;
  color: white;
  text-align: center;
  padding: 20px 25px;
  text-decoration: none;
}

li a:hover {
  background-color: #111;
}

.sidebar {
  width: 200px;
  background-color: #222;
  color: white;
  padding-top: 20px;
}

.sidebar img {
  width: 100%;
  max-width: 150px; /* Adjust the size as needed */
  display: block;
  margin: 0 auto;
  border-radius: 50%;
}

.sidebar-link {
  display: block;
  color: white;
  text-align: center;
  padding: 20px;
  text-decoration: none;
  transition: background-color 0.3s;
}

.sidebar-link:hover {
  background-color: #111;
}

footer{
  position: fixed;
  left: 0;
  bottom: 0;
  width: 100%;
  background-color: gray;
  color: white;
  text-align: center;
}


</style>
