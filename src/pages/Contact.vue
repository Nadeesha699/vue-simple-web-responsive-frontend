<script setup></script>

<template>
  <div id="contact" class="contact">
    <div class="sub-footer">
      <img src="../assets/images/letter-n.png" style="width: 100px; height: 100px;"/>
      <div class="sub-footer2">
        <h1>CONTACT</h1>
        <label>nadeesharuwandima@gmail.com</label>
        <label>+94 7117 6232</label>
      </div>
    </div>
    <label>disgned by:- nadeesharuwandima@gmail.com</label>
  </div>
</template>

<style scoped>
.contact{
    background-color: rgb(255, 255, 255);
    padding: 2%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    padding: 5%;
    gap: 50px;
    margin-top: 5%;
    box-shadow: 0px 0px 10px black;
    width: 100%;
}

.sub-footer{
    display: flex;
    flex-direction: row;
    gap: 5%;
    justify-content: center;
    align-items: center;
}
.sub-footer2{
display: flex;
flex-direction: column;
}

h1{
  letter-spacing: 4px;
}
label{
  font-weight: bold;
  letter-spacing: 1px;
}
</style>
