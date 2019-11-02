<template>
  <div class="home">
    <navbar></navbar>
    <chakravyuh-title></chakravyuh-title>
    <countdown-timer></countdown-timer>
  </div>
</template>

<style media="screen">
  body{
    background-image: url('../assets/images/galaxy.jpg');
    background-size: cover;
    background-repeat: no-repeat;
    background-position: center;
  }

</style>

<script>
// @ is an alias to /src
import navbar from "@/components/navbar.vue"
import CountdownTimer from "@/components/countdownTimer.vue"
import ChakravyuhTitle from "@/components/ChakravyuhTitle.vue"

export default {
  name: 'home',
  components: {
    'countdown-timer' : CountdownTimer,
    'navbar' : navbar,
    'chakravyuh-title' : ChakravyuhTitle
  }

}
</script>
