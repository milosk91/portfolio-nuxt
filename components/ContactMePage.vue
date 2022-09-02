<template>
  <div>
    <NavBar />
    <div class="container">
      <div class="right">
        <div class="image">
          <img src="../static/ja.png" class="img" alt="" />
        </div>
      </div>

      <div class="left">
        <div class="square">
          <span></span>
          <span></span>
          <span></span>
          <div class="content">
            <h2>Contact Me</h2>
            <p>
              Thank you for visiting my design portfolio. If you’d like to see
              more or would like to get in touch, my contact information is
              provided below.
            </p>
            <div class="contact">
              <svg
                class="svg"
                xmlns="http://www.w3.org/2000/svg"
                viewBox="0 0 512 512"
              >
                <a href="mailto:milos.koruga.1@gmail.com" target="_blank">
                  <!--! Font Awesome Pro 6.1.1 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license (Commercial License) Copyright 2022 Fonticons, Inc. -->
                  <path
                    d="M464 64C490.5 64 512 85.49 512 112C512 127.1 504.9 141.3 492.8 150.4L275.2 313.6C263.8 322.1 248.2 322.1 236.8 313.6L19.2 150.4C7.113 141.3 0 127.1 0 112C0 85.49 21.49 64 48 64H464zM217.6 339.2C240.4 356.3 271.6 356.3 294.4 339.2L512 176V384C512 419.3 483.3 448 448 448H64C28.65 448 0 419.3 0 384V176L217.6 339.2z"
                  />
                </a>
              </svg>
              <svg
                class="svg"
                xmlns="http://www.w3.org/2000/svg"
                viewBox="0 0 448 512"
              >
                <a
                  href="https://www.linkedin.com/in/milos-koruga-0ba958206/"
                  target="_blank"
                >
                  <!--! Font Awesome Pro 6.1.1 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license (Commercial License) Copyright 2022 Fonticons, Inc. -->
                  <path
                    d="M416 32H31.9C14.3 32 0 46.5 0 64.3v383.4C0 465.5 14.3 480 31.9 480H416c17.6 0 32-14.5 32-32.3V64.3c0-17.8-14.4-32.3-32-32.3zM135.4 416H69V202.2h66.5V416zm-33.2-243c-21.3 0-38.5-17.3-38.5-38.5S80.9 96 102.2 96c21.2 0 38.5 17.3 38.5 38.5 0 21.3-17.2 38.5-38.5 38.5zm282.1 243h-66.4V312c0-24.8-.5-56.7-34.5-56.7-34.6 0-39.9 27-39.9 54.9V416h-66.4V202.2h63.7v29.2h.9c8.9-16.8 30.6-34.5 62.9-34.5 67.2 0 79.7 44.3 79.7 101.9V416z"
                  />
                </a>
              </svg>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { Vue, Component } from "vue-property-decorator";
import NavBar from "~/components/NavBar.vue";

@Component({
  components: {
    NavBar,
  },
})
export default class ContactMePage extends Vue {
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
  display: flex;
  width: 100%;
  justify-content: space-around;
  margin-top: 8rem;
}
@media screen and (max-width: 990px) {
  .container {
    display: flex;
    flex-direction: column;
  }
}
.content {
  max-width: 400px;
  color: rosybrown;
  text-align: center;
  display: flex;
  flex-direction: column;
  font-family: "Roboto", sans-serif;
}

.square {
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
  position: relative;
  color: rosybrown;
  text-align: center;
  transition: 0.5s;
  font-size: 1rem;
  display: flex;
  flex-direction: column;
}

.img {
  max-width: 500px;
  max-height: 500px;
  border: 1px solid #ececec;
  border-radius: 68% 33% 53% 27% / 91% 64% 86% 39%;
}
@media screen and (max-width: 990px) {
  .img {
    max-width: 100%;
    max-height: 100%;
    width: 300px;
    height: 350px;
    display: flex;
    margin: auto;
  }
}
.image {
  display: flex;
  justify-content: center;
}
.contact {
  display: flex;
  justify-content: center;
}
p {
  font-size: 1.5rem;
  margin-top: 0.25rem;
  font-weight: 300;
}
@media screen and (max-width: 990px) {
  p {
    margin-top: 0;
    width: 250px;
    font-size: 1.2rem;
  }
}
h2 {
  font-size: 2rem;
  font-weight: 400;
}
.svg {
  max-width: 2.5rem;
  fill: rosybrown;
  opacity: 1;
  margin-right: 1rem;
}
@media screen and (max-width: 990px) {
  .svg {
    width: 1.5rem;
  }
}
.svg:hover {
  opacity: 0.6;
  cursor: pointer;
  transform: scale(1.1);
}
path {
  fill: rosybrown;
}
</style>
