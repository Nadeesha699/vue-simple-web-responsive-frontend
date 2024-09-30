<script setup></script>

<template>
  <div id="about" class="about">
    <div style="order: 2" class="forOrder1">
      <h1><span>A</span>bout</h1>
      <p>
        Lorem ipsum, dolor sit amet consectetur adipisicing elit. In praesentium
        vitae soluta neque cum nemo? Error, voluptatem, eveniet assumenda dolore
        doloremque hic vitae illo excepturi blanditiis est, dolorum porro modi?
      </p>
    </div>
    <div class="forOrder2">
      <img
        src="../assets/images/make-up.png"
        style="
          width: 400px;
          height: 400px;
          border-top-left-radius: 50px;
          border-bottom-right-radius: 50px;
        "
      />
    </div>
  </div>
</template>

<style lang="css" scoped>
h1 {
  color: rgb(0, 0, 0);
  font-size: 50px;
  text-shadow: 20px 10px 10px black;
}
.about {
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: space-around;
  padding: 10%;
  gap: 20%;
}

span {
  color: rgb(255, 0, 89);
}

p {
  font-size: 15px;
  letter-spacing: 4px;
  font-family: Arial, Helvetica, sans-serif;
}

/* Extra small devices (phones, less than 576px) */
@media (max-width: 575.98px) {
  .about {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: space-around;
  padding: 10%;
  gap: 20%;
}

.forOrder1{
  order: 1;
}

.forOrder2{
  order: 2;
}
}

/* Small devices (tablets, 576px and up) */
@media (min-width: 576px) and (max-width: 767.98px) {
  .about {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: space-around;
  padding: 10%;
  gap: 20%;
}

.forOrder1{
  order: 1;
}

.forOrder2{
  order: 2;
}
}
</style>
