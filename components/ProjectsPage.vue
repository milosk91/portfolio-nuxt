<template>
  <div>
    <NavBar />
    <div class="container">
      <div class="top">
        <div class="content">
          <h2>Apartments App</h2>
          <p>Web Design</p>
        </div>
        <a
          href="https://xd.adobe.com/view/35270ab6-97d6-4722-975d-cbceb7282a35-6074/"
          target="_blank"
        >
          <img src="../static/apartmants.png" class="img apartments" />
        </a>
        <div class="content">
          <h2>Change Career App</h2>
          <p>Web Design</p>
          <a
            href="https://www.figma.com/proto/lONAJpf25uSjStZIo2KVi6/Career-Change-Hi-Fi-Prototype?page-id=0%3A1&node-id=1%3A2&viewport=530%2C321%2C0.31&scaling=min-zoom&starting-point-node-id=1%3A428"
            target="_blank"
          >
            <img src="../static/change-career.png" class="img-mobile" />
          </a>
        </div>
      </div>
      <div class="bottom">
        <div class="content">
          <h2>SteakHouse Book A Table App</h2>
          <p>Web Design</p>
          <a
            href="https://www.figma.com/proto/qOgZrXUisL8sFTwacG7xU1/SteakHouse-Table-Reservation?page-id=0%3A1&node-id=113%3A96&viewport=427%2C65%2C0.09&scaling=scale-down&starting-point-node-id=113%3A215&show-proto-sidebar=1"
            target="_blank"
          >
            <img src="../static/steakhouse.png" class="img-mobile steakhouse" />
          </a>
        </div>
        <div class="content">
          <h2>Futureworks Pricing Page</h2>
          <p>Web Design & Coding</p>
          <a href="https://www.futureworks.com/en/price" target="_blank">
            <img
              src="../static/futureworks-pricing-page.png"
              class="img-mobile futureworks"
            />
          </a>
        </div>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { Vue, Component } from 'vue-property-decorator'
import NavBar from '~/components/NavBar.vue'

@Component({
  components: {
    NavBar,
  },
})
export default class Projects extends Vue {
  /* Props */
  /* State */
  /* Data */
  /* Hooks */
  /* Methods */
  /* Computed */
  /* Watchers */
}
</script>

<style scoped>
.container {
  width: 100%;
  display: flex;
  justify-content: space-around;
  margin: auto;
  margin-top: 5rem;
}
@media screen and (max-width: 990px) {
  .container {
    display: flex;
    flex-direction: column;
  }
}

.square {
  position: relative;
  max-width: 500px;
  max-height: 500px;
  display: flex;
  justify-content: center;
  align-items: center;
}
@media screen and (max-width: 990px) {
  .square {
    max-width: 100%;
    width: 350px;
    height: 350px;
    display: flex;
    margin: 50px auto;
  }
}

.square span:nth-child(1) {
  position: absolute;
  width: 100%;
  height: 100%;
  border: 2px solid rosybrown;
  border-radius: 38% 63% 63% 37% / 41% 44% 56% 59%;
  transition: 0.5s;
  animation: animate 6s linear infinite;
}

/* .square:hover span:nth-child(1) {
  border: none;
  background: rosybrown;
} */

.square span:nth-child(2) {
  position: absolute;
  width: 100%;
  height: 100%;
  border: 2px solid #ecb;
  border-radius: 38% 63% 63% 37%/41% 44% 56% 59%;
  transition: 0.5s;
  animation: animate2 4s linear infinite;
}

.square span:nth-child(3) {
  position: absolute;
  width: 100%;
  height: 100%;
  border: 2px solid #ecc;
  border-radius: 38% 63% 63% 37%/41% 44% 56% 59%;
  transition: 0.5s;
  animation: animate 10s linear infinite;
}
.square span:nth-child(4) {
  position: absolute;
  width: 100%;
  height: 100%;
  border: 2px solid #ecc;
  border-radius: 68% 33% 23% 67%/11% 14% 76% 89%;
  transition: 0.5s;
  animation: animate 10s linear infinite;
}

@keyframes animate {
  0% {
    transform: rotate(0deg);
  }

  100% {
    transform: rotate(360deg);
  }
}

@keyframes animate2 {
  0% {
    transform: rotate(360deg);
  }

  100% {
    transform: rotate(0deg);
  }
}

.content {
  position: relative;
  color: rosybrown;
  text-align: center;
  transition: 0.5s;
  font-size: 16px;
  display: flex;
  flex-direction: column;
  font-family: 'Roboto', sans-serif;
  margin-top: 5rem;
}
@media screen and (max-width: 990px) {
  .content {
    margin-top: 2rem;
  }
}

.apartments {
  max-width: 500px;
  max-height: 500px;
  border: 1px solid #ececec;
  border-radius: 38% 63% 63% 37% / 41% 44% 56% 59%;
  opacity: 1;
  transition: transform 0.7s;
}
@media screen and (max-width: 990px) {
  img {
    width: 350px;
    display: flex;
    margin: 30px auto;
  }
}
.img-mobile {
  width: 250px;
  height: 600px;
  border: 1px solid #ececec;
  border-radius: 63% 38% 36% 72% / 31% 54% 36% 49%;
  opacity: 1;
  transition: transform 0.7s;
}
.apartments:hover {
  opacity: 0.6;
  transform: scale(1.05);
}
.img-mobile:hover {
  opacity: 0.6;
  transform: scale(1.05);
}
.steakhouse {
  border-radius: 33% 58% 76% 42% / 11% 14% 36% 39%;
}
.futureworks {
  max-width: 500px;
  width: 100%;
  max-height: 500px;
  border: 1px solid #ececec;
  border-radius: 71% 43% 53% 17% / 21% 34% 46% 69%;
  opacity: 1;
  transition: transform 0.7s;
}

p {
  font-size: 1rem;
  margin-top: 0.25rem;
  font-weight: 300;
}
h2 {
  font-size: 2rem;
  font-weight: 400;
}
</style>
