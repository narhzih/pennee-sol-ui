<template>
  <div class="container">
    <h3 class="text-center c-head">Cash flow is king</h3>
    <div class="row">
      <div class="col-md-6">
        <div class="card card--input text-start">
          <h4>Current cashflow</h4>
          <h2>How much do you make?</h2>
          <form action="#" >
            <input type="number" placeholder="Enter amount" class="form-control" v-model="amount">
          </form>
        </div>
      </div>
      <div class="col-md-6">
        <div class="card card--output text-start">
          <h4>With pennee</h4>
          <h2>How much you'll make</h2>
          <h1 class="c-result">{{calculated_amount}}</h1>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Calculator",
  data() {
    return {
      amount: 0,
      calculated_amount: 0.00
    }
  }
}
</script>

<style scoped>
  .c-head {
    font: normal normal 800 50px/74px Mulish;
    letter-spacing: 0px;
    color: #021C34;
    opacity: 1;
    margin-bottom: 5rem;
  }
  .card {
    padding: 3rem;
    min-height: 30rem !important;
  }
  .card--input {
    background-color: #FEF5F2;
  }
  .card--output {
    background-color: #EFEAFF;
  }
  .card > h4 {
    font: normal normal bold 26px/35px Mulish;
    letter-spacing: 0px;
    color: #021C34;
    opacity: 1;
  }
  .card > h2 {
    font: normal normal 800 43px/55px Mulish;
    letter-spacing: 0px;
    color: #021C34;
    opacity: 1;

  }

  .card > form {
    position: absolute;
    width: 85%;
    left: 50%;
    top: 80%;
    transform: translateX(-50%);
  }
  .c-result {
    position:absolute;
    top: 75%;
    text-align: left;
    font: normal normal 800 70px/90px Mulish;
    letter-spacing: 0px;
    color: #021C34;
    opacity: 1;

  }
</style>