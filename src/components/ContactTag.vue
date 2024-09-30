<template>
  <div class="contact-tag">
    <a href="#contact"
      ><img
        src="../assets/images/telephone.png"
        style="width: 30px; height: 30px; transition: all 0.5s ease-in-out"
    /></a>
  </div>
</template>

<style scoped>
.contact-tag {
  background-color: rgb(255, 255, 255);
  width: 50px;
  height: 50px;
  border-radius: 50px;
  position: fixed;
  bottom: 5%;
  right: 5%;
  display: flex;
  align-items: center;
  justify-content: center;
  box-shadow: 0px 0px 10px black;
  transition: all 0.5s ease-in-out;
}

.contact-tag:hover {
  background-color: rgb(255, 0, 115);
  box-shadow: 0px 0px 0px black;
}

img:hover {
  content: url(../assets/images/chevron.png);
}
</style>
