<template>
  <section class="">
    <section>
      <v-img class="bg" src="/bg.jpg">
        <section class="bg-content white--text">
          <div class="my-text animated tada">START, LEARN, SUCCEED</div>
          <div>
            <v-btn to="/user" round large class="white navbarBg--text">Start your future</v-btn>
          </div>
        </section>
      </v-img>
    </section>
  </section>
</template>

<style lang="scss" scoped>
  .bg {
    text-align: center;
    height: 678px;
    @media (min-width: 1450px) {
      height: 739px;
    }
    @media (min-width: 1500px) {
      height: 754px;
    }
    @media (min-width: 1700px) {
      height: 850px;
    }
    @media (min-width: 1800px) {
      height: 904px;
    }
    @media (min-width: 1850px) {
      height: 1017px;
    }
    @media (min-width: 2150px) {
      height: 1130px;
    }
    @media (min-width: 2300px) {
      height: 1358px;
    }
    @media (min-width: 2800px) {
      height: 1650px;
    }
    @media (min-width: 3400px) {
      height: 2033px;
    }
    @media (min-width: 5400px) {
      height: 2710px;
    }
  }

  .bg-content {
    display: block;
    position: absolute;
    top: 55%;
    left: 50%;
    transform: translate(-50%, -50%);
    font-size: 5em;
    font-weight: bolder;
    @media (max-width: 425px) {
      top: 46%;
      font-size: 4em;
    }
    @media (max-width: 375px) {
      top: 45%;
      font-size: 3em;
    }
  }

  .v-btn {
    font-size: 12px;
    font-weight: 900;
    width: 200px;
    height: 50px;
    border-radius: 0 25px;
  }

  .v-btn:hover {
    background-color: #188b73 !important;
    color: white !important;
    border: solid white 2px;
  }

  .my-text {
    text-shadow: 0px 15px 5px rgba(0, 0, 0, 0.1), 10px 20px 5px rgba(0, 0, 0, 0.05), -10px 20px 5px rgba(0, 0, 0, 0.05);
  }
</style>

<script>
  export default {

  }
</script>


