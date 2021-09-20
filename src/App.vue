<template>
  <div id="app">
    <div class="app-banner">
      <div class="container">
        <div class="row d-flex align-items-center">
          <div class="col-md-6 text-start">
            <h1 class="text-start app-banner__header">
              Growth partner for
              small businesses
            </h1>
            <p class="app-banner__sub">Enjoy asset loans, automated business management, and business reports summarized in plain English.</p>
            <a href="#" class="app-banner__button">Get Early Access Now</a>
          </div>

          <div class="col-md-6">
            <img src="@/assets/images/figure_1.png">
          </div>
        </div>
        <img src="@/assets/images/chat_icon.svg" class="app-banner__chat-icon" alt="bottom-icon">
      </div>
    </div>
    <div class="app__calculator">
      <calculator></calculator>
    </div>
  </div>
</template>

<script>


import Calculator from "./components/Calculator";
export default {
  name: 'App',
  components: {
    Calculator

  }
}
</script>

<style >
body {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  /*color: #2c3e50;*/
  /*margin-top: 60px;*/
}

.app-banner__chat-icon {
  position: absolute;
  left: 95%;
  top: 70%;
  transform: translateX(-95%);
}

.app-banner {
  position: relative;
  padding: 5rem 20rem;
  min-height: 100vh;
  width: 100%;
  background: transparent linear-gradient(180deg, #EEE8FE 0%, #4B397E00 100%) 0% 0% no-repeat padding-box;

}
.app-banner__header {
  color: #021C34;
  font-weight: 800;
  font-size: 70px;
  font-family: 'Mulish', sans-serif;
  letter-spacing: -2.1px;
}

.app-banner__sub {
  display: inline-block;
  margin-top: 1rem;
}
.app-banner__button {
  background: #9672FB 0% 0% no-repeat padding-box;
  border-radius: 5px;
  opacity: 1;
  padding: 1rem;
  text-decoration: none;
  color: #ffffff;
  display: inline-block;
  margin-top: 1rem;
}

.app-banner__button:hover {
  color: #ffffff;
}
</style>
