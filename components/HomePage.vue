<template>
  <div>
    <NavBar />
    <div class="container">
      <div class="image">
        <img src="../static/ja.png" class="img" alt="person" />
      </div>

      <div class="square">
        <span></span>
        <span></span>
        <span></span>
        <div class="content">
          <h2>Hey there!</h2>
          <p>
            My name is Milos. I’m a creative and passionate Front-End Developer
            and Web Designer based in Oslo, Norway.
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { Vue, Component } from 'vue-property-decorator'
import NavBar from '../components/NavBar.vue'

@Component({
  components: {
    NavBar,
  },
})
export default class HomePage extends Vue {
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
body {
  display: flex;
  justify-content: center;
  align-items: center;
  /* background: #f6f6f6; */
}

.container {
  display: flex;
  width: 100%;
  justify-content: center;
}
@media screen and (max-width: 990px) {
  .container {
    display: flex;
    flex-direction: column-reverse;
  }
}
p {
  font-size: 2rem;
  margin-top: 0.25rem;
  font-weight: 300;
}
@media screen and (max-width: 990px) {
  p {
    font-size: 1.5rem;
    width: 230px;
    margin-top: 0;
  }
}
h2 {
  font-size: 3.5rem;
  font-weight: 400;
}
@media screen and (max-width: 990px) {
  h2 {
    font-size: 2rem;
  }
}

.square {
  margin-top: 100px;
  margin-left: 100px;
  position: relative;
  width: 500px;
  height: 500px;
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
  max-width: 400px;
  color: rosybrown;
  text-align: center;
  display: flex;
  flex-direction: column;
  font-family: 'Roboto', sans-serif;
}
.right {
  width: 50%;
  height: 100%;
}
.img {
  margin-top: 100px;
  max-width: 500px;
  max-height: 500px;
  border-radius: 38% 63% 63% 37% / 41% 44% 56% 59%;
}
@media screen and (max-width: 990px) {
  .img {
    max-width: 100%;
    max-height: 100%;
    width: 350px;
    height: 350px;
    display: flex;
    margin: 2rem auto;
  }
}
</style>
