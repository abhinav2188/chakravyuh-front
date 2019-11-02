<template lang="html">
  <div class="relative subpixel-antialiased lead rounded shadow">
    <img class="md:w-16 md:h-16 w-12 h-12 rounded-full lead-img shadow-md" :src="profileSrc" alt="">
    <div class="flex md:p-4 p-3 mt-10 mb-1">
      <div class='rank flex flex-col'>
        <span class="md:text-xsm text-2xsm font-bold self-center">Rank</span>
        <span class="font-bold self-center md:text-2xl text-lg">{{rank}}</span>
      </div>
      <span class="self-end name md:text-md text-xm">{{name}}</span>
      <div class='points flex flex-col'>
        <span class="md:text-xsm text-2xsm font-bold self-center">Points</span>
        <span class="font-bold self-center md:text-2xl text-lg">{{points}}</span>
      </div>

    </div>
  </div>
</template>

<script>
export default {
  props:{
    pid: {
      type : Number,
    },
    photoSrc :{
      type: String,
    },
    name :{
      type : String,
      required : true
    },
    points : {
      type : Number,
      required : true
    },
    rank : {
      type : Number,
      required : true
    }
  }

}
</script>

<style lang="css" scoped>
  .text-xsm{
    font-size: .5rem;
  }
  .text-2xsm{
    font-size: .4rem;
  }
  .lead{
    background-image: linear-gradient(to bottom,#77ff77,#99ff99);
  }
  .lead-img{
    position : absolute;
    top:0;
    left : 50%;
    transform: translate(-50%,-50%);
  }
  .rank{
    flex:2;
  }
  .name{
    flex:6;
  }
  .points{
    flex:2;
  }
</style>
