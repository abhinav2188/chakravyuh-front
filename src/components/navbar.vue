<template lang="html">
  <!-- <div class="flex container text-gray-300 block h-8 mr-0">
      <ul class="float-left inline-block">
        <li class="font-bold text-lg inline-block">
          <a href="#">Chakravyuh</a>
        </li>
        <li class="inline-block">
          <a href="#">Dashboard</a>
        </li>
      </ul>
      <ul class="float-right inline-block">
        <li>
          <a href="#">Login</a>
        </li>
      </ul>
  </div> -->

  <div class="flex justify-between w-4/5 mx-auto text-sm align-middle text-gray-500 border-b">
    <div class="flex align">
      <a href="#" class="p-1 mr-4 hover:text-white ">Chakravyuh</a>
      <a href="#" class='p-1 hover:text-white'>Dashboard</a>
    </div>

    <div class="flex">
      <a href="#" class='p-1 hover:text-white'>Login</a>
    </div>
  </div>
  <!-- <nav class="flex items-center justify-between flex-wrap p-2">
    <div class="flex text-white mr-6">
      <a class="font-semibold text-xl tracking-tight m-3">Chakravyuh</a>
      <a class="font-base m-2 mt-4" href="#">Dashboard</a>

    </div>
    <div class="block lg:hidden">
      <button class="flex items-center px-3 py-2 border rounded text-teal-200 border-teal-400 hover:text-white hover:border-white">
        <svg class="fill-current h-3 w-3" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><title>Menu</title><path d="M0 3h20v2H0V3zm0 6h20v2H0V9zm0 6h20v2H0v-2z"/></svg>
      </button>
    </div>
    <div class=" lg:flex lg:items-center lg:w-auto">
      <div class="text-sm lg:flex-grow ">
        <a href="#" class="block m-2 mt-4 lg:inline-block lg:mt-0 text-teal-200 hover:text-white mr-4">
          Login
        </a>
      </div>
    </div>
  </nav> -->

</template>

<script>
export default {
}
</script>

<style lang="css" scoped>
#topnav{
  top : 1rem;
  left : 50%;
  transform : translateX(-50%);
}
</style>
