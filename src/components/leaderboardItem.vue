<template lang="html">
  <div class="flex p-3 border-b ">
    <span class='rank self-center md:text-lg text-xm'>{{rank}}</span>
    <div class="profile flex ">
      <div class="profile-img ">
        <img class="md:w-10 md:h-10 w-8 h-8 border rounded-full inline-block  shadow" :src="photoSrc" alt="">
      </div>
      <span class="profile-name text-xs self-center text-left ">{{name}}</span>
      <div class="profile-log self-center">

      </div>
    </div>
    <span class='points self-center md:text-lg text-sm '>{{points}}</span>
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
.profile{
  flex:7;
}
.profile-name{
  flex: 9;
}
.profile-img{
  flex:2;
}
.profile-log{
  flex:2;
}
.points{
  flex:2
}
.rank{
  flex:1
}
</style>
