<script setup>
function clickAbout() {}
</script>

<template>
  <div class="home">
    <div style="width: 50%; padding-left: 9%">
      <h1><span>PINK</span> MOON SHOP</h1>
      <a href="#about">see more</a>
    </div>
    <div class="home-background">
      <img src="../assets/images/sakura.png" style="width: 69%; height: 69%" />
    </div>
  </div>
</template>

<style scoped>
h1 {
  color: rgb(0, 0, 0);
  font-size: 50px;
  text-shadow: 20px 10px 10px black;
}
span {
  color: rgb(255, 0, 89);
}

.home {
  margin-top: 8%;
  display: flex;
  flex-direction: row;
  width: 100%;
  justify-content: center;
  align-items: center;
}

a {
  border-style: solid;
  border-color: black;
  border-radius: 20px;
  background-color: rgba(255, 255, 255, 0);
  padding: 8px;
  cursor: pointer;
  border-width: 2px;
  letter-spacing: 5px;
  transition: all 0.5s ease-in-out;
  text-decoration: none;
  color: black;
}

a:hover {
  background-color: rgb(255, 0, 89);
  color: white;
  box-shadow: 10px 10px 10px black;
  border-style: hidden;
}

.home-background {
  width: 50%;
  padding-top: 6%;
}

/* Extra small devices (phones, less than 576px) */
@media (max-width: 575.98px) {
  .home {
    display: flex;
    flex-direction: column;
    justify-content: space-around;
    align-items: center;
    gap: 50px;
    padding: 20px;
  }
}

/* Small devices (tablets, 576px and up) */
@media (min-width: 576px) and (max-width: 767.98px) {
  .home {
    display: flex;
    flex-direction: column;
    justify-content: space-around;
    align-items: center;
    gap: 50px;
    padding: 20px;
  }
}

</style>
