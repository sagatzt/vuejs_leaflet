<template>
  <div class="app">
    <nav class="navbar navbar-expand-sm navbar-dark bg-custom">
      <div class="container-fluid">
        <a class="navbar-brand" href="#">Ejemplo Leaflet - Fullstack</a>
        <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarSupportedContent">
          <ul class="navbar-nav mb-2 mb-lg-0">
            <li class="nav-item">
              <router-link to="/" class="nav-link ">Home</router-link>
            </li>
            <li class="nav-item">
              <router-link to="/about" class="nav-link">About</router-link>
            </li>
            <li class="nav-item">
              <router-link to="/map" class="nav-link">Mapa</router-link>
            </li>            
          </ul>
        </div>
      </div>
    </nav>    
  </div>

  <router-view/>
</template>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

.navbar.bg-custom{
   background-color: #258565;
   margin-bottom:30px;
  -webkit-box-shadow: 0px 10px 5px 5px rgba(156,214,202,1);
  -moz-box-shadow: 0px 10px 5px 5px rgba(156,214,202,1);
  box-shadow: 0px 10px 5px 5px rgba(156,214,202,1);
  border-bottom: 7px solid rgb(8, 83, 71);
}

.navbar-nav{
  
}

#nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
