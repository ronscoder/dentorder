<template>
  <!-- <div class="headbar">
      <img id="brand" alt="Dentorder logo" :src="logo">
      <a href>
        <h3>DentOrder</h3>
      </a>
      <div class="menu">
        <a href>Home</a>
        <a href>Dental Lab</a>
        <a href>Dental Store</a>
        <a href>Offer</a>
        <a href>Dental Update</a>
        <a href>About</a>
      </div>
  </div>-->
  <div>
    <b-navbar toggleable="lg" type="dark" variant="dark" :sticky="true" class="navbar">
      <b-navbar-brand href="#">
        <div id="navbrand">
          <img id="logo" :src="logo">
          <div>
            Dentorder
            <br>
            <i>
              <small>Dental Supplier</small>
            </i>
          </div>
        </div>
      </b-navbar-brand>

      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

      <b-collapse id="nav-collapse" class="ml-auto" is-nav>
        <b-navbar-nav>
          <b-nav-item href="#">Home</b-nav-item>
          <b-nav-item href="#">Dental Store</b-nav-item>
          <b-nav-item href="#">Dental Lab</b-nav-item>
          <b-nav-item href="#">Offer</b-nav-item>
          <b-nav-item href="#">Dental Update</b-nav-item>
          <b-nav-item href="#">About</b-nav-item>
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
  </div>

</template>

<script>
import logo from "../assets/logo.png";
export default {
  data: function() {
    return {
      logo: logo
    };
  }
};
</script>

<style>
#logo {
  width: 60px;
  height: 60px;
}
.navbar {
  width: 100%;
  position: fixed; 
}

#navbrand {
  widows: 100px;
  display: flex;
  flex-direction: row;
}
</style>


