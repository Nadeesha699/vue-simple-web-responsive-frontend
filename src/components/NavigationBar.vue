<script>
export default {
  data() {
    return {
      visibleMenu: false,
    };
  },

  methods: {
    visibleMenuButton() {
      this.visibleMenu = !this.visibleMenu;
    },
  },
};
</script>

<template>
  <div class="nav-main">
    <div class="sub-nav1">
      <img alt="logo" src="../assets/images/letter-n.png" />
    </div>
    <div class="sub-nav2" @click="visibleMenuButton">
      <img src="../assets/images/menu-bar.png" class="menu" />
    </div>
    <div v-if="visibleMenu" class="mobileMenu">
        <img  src="../assets/images/crossed.png" class="closeMenu" @click="visibleMenuButton"/>
      <a href="../pages/Home.vue" style="color: rgb(255, 0, 89)">Home</a>
      <a href="#service" @click="visibleMenuButton">Service</a>
      <a href="#about" @click="visibleMenuButton">About</a>
      <a href="#contact" @click="visibleMenuButton">Contact</a>
    </div>
    <div class="sub-nav3">
      <a href="../pages/Home.vue" style="color: rgb(255, 0, 89)">Home</a>
      <a href="#service">Service</a>
      <a href="#about">About</a>
      <a href="#contact">Contact</a>
    </div>
  </div>
</template>

<style scoped>
.nav-main {
  /* background-color: red; */
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: space-between;
  width: 100%;
  box-shadow: 0px 0px 10px black;
  position: fixed;
  top: 0;
  background-color: white;
}

.sub-nav1 {
  display: flex;
  flex-direction: row;
  width: 60%;
  /* background-color: yellow; */
  padding-left: 2%;
}

.sub-nav2 {
  display: none;
  flex-direction: row;
  width: 40%;
  justify-content: right;
  padding-right: 2%;
}

.sub-nav3 {
  display: flex;
  flex-direction: row;
  width: 40%;
  /* background-color: green; */
  justify-content: space-around;
}

a {
  color: rgb(0, 0, 0);
  text-decoration: none;
  text-transform: uppercase;
  letter-spacing: 3px;
  font-weight: bold;
  line-height: 10px;
  transition: all 0.2s ease-in-out;
}

a:hover {
  text-shadow: 10px 10px 5px black;
}
img {
  width: 70px;
  height: 70px;
}

.mobileMenu {
  background-color: rgb(255, 129, 150);
  width: 100%;
  height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: space-around;
  position: fixed;
  top: 0;
  bottom: 0;
  left: 0;
  right: 0;
  align-items: center;
}

.closeMenu{
    cursor: pointer;
    transition: all 0.2s ease-in-out;
}

.closeMenu:hover{
   background-color: white;
   border-radius: 50px;
}

/* Extra small devices (phones, less than 576px) */
@media (max-width: 575.98px) {
  .sub-nav2 {
    display: flex;
  }
  .sub-nav3 {
    display: none;
  }
}

/* Small devices (tablets, 576px and up) */
@media (min-width: 576px) and (max-width: 767.98px) {
  .sub-nav2 {
    display: flex;
  }
  .sub-nav3 {
    display: none;
  }
}

/* Medium devices (small laptops, 768px and up) */
@media (min-width: 768px) and (max-width: 991.98px) {
  .sub-nav2 {
    display: flex;
  }
  .sub-nav3 {
    display: none;
  }
}
</style>
