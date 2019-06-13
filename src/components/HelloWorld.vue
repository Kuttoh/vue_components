<template>

  <div id="app" class="container">
    This is the message to display: {{msg}}

    <welcome></welcome>

  <task-list></task-list>

    <message title="Hello world" body="Lorem ipsum dolor sit amet, consectetur adipiscing elit."></message>

    <message title="Some Message" body="Some long incomprehensible text."></message>

    <coupon @applied="onCouponApplied"></coupon>

    <h1 v-if="couponApplied">Enjoy your KES 500 free ride!</h1>

<!--    <modal></modal>-->

<!--    <button @click="showModal=true">Show Modal</button>-->


    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/bulma/0.7.5/css/bulma.css">

  </div>

</template>

<script>
 import welcome from "./welcome"
 import newTask from "./newTask"
 import taskList from "./taskList"
 import message from "./message"
 import modal from "./modal"
 import coupon from "./coupon"

export default {
  name: 'app',
  components: {taskList, newTask, welcome, message, modal, coupon},
  data () {
    return {
      msg: 'Lion King',
      couponApplied: false
    }
  },

  methods:{
    onCouponApplied(){
      this.couponApplied = true
    }
  }
}

</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
