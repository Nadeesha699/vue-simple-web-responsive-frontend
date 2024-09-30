<script>
export default {
  data() {
    return {
      data: [
        {
          serviceName: "Beauty",
          discription:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Fugiat quibusdam alias laudantium officiis aliquam. ",
          image: "../src/assets/images/anti-age.png",
        },
        {
          serviceName: "Makup",
          discription:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Fugiat quibusdam alias laudantium officiis aliquam.",
          image: "../src/assets/images/makeup-brushes.png",
        },
        {
          serviceName: "Happy",
          discription:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Fugiat quibusdam alias laudantium officiis aliquam.",
          image: "../src/assets/images/girl.png",
        },
      ],
    };
  },
};
</script>

<template>
  <div id="service" class="service">
    <h1>Service</h1>
    <div class="card-ground">
      <div v-for="e in data" class="card">
        <label class="serviceName">{{ e.serviceName }}</label>
        <label class="discription">{{ e.discription }}</label>
        <img
          :src="e.image"
          alt="image"
          style="width: 100px; height: 100px; order: 2"
        />
      </div>
    </div>
  </div>
</template>

<style scoped>
h1 {
  color: rgb(0, 0, 0);
  font-size: 50px;
  text-shadow: 20px 10px 10px black;
}
.service {
  padding-top: 11%;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: space-around;
}

span {
  color: rgb(255, 0, 89);
}

.card-ground {
  display: flex;
  flex-direction: row;
  justify-content: space-around;
  align-items: center;
  gap: 10%;
}

.card {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  background-color: rgb(255, 0, 89);
  width: 300px;
  height: 350px;
  padding: 2%;
  border-radius: 20px;
  box-shadow: 10px 10px 10px black;
  gap: 5%;
}

.serviceName {
  order: 1;
  font-size: 30px;
  color: white;
  letter-spacing: 3px;
  font-family: "Lucida Sans", "Lucida Sans Regular", "Lucida Grande",
    "Lucida Sans Unicode", Geneva, Verdana, sans-serif;
  text-transform: uppercase;
}

.discription {
  order: 3;
  text-align: center;
  font-size: 13px;
  letter-spacing: 3px;
  color: white;
}

/* Extra small devices (phones, less than 576px) */
@media (max-width: 575.98px) {
  .card-ground {
    display: flex;
    flex-direction: column;
    justify-content: space-around;
    align-items: center;
    gap: 20px;
  }

  .card {
    width: 200px;
    height: 250px;
  }
}

/* Small devices (tablets, 576px and up) */
@media (min-width: 576px) and (max-width: 767.98px) {
  .card-ground {
    display: flex;
    flex-direction: column;
    justify-content: space-around;
    align-items: center;
    gap: 20px;
  }

  .card {
    width: 200px;
    height: 250px;
  }
}

/* Medium devices (small laptops, 768px and up) */
@media (min-width: 768px) and (max-width: 991.98px) {
  .card-ground {
    display: flex;
    flex-direction: column;
    justify-content: space-around;
    align-items: center;
    gap: 20px;
  }

  .card {
    width: 200px;
    height: 250px;
  }
}
</style>
