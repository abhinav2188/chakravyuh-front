<template lang="html">
  <div class="lg:w-3/4  mx-auto bg-gray-100 text-gray-900 lg:p-6 md:p-4 p-0 lg:pl-24 lg:pr-24 rounded shadow max-h-screen overflow-scroll subpixel-antialiased leaderboard">
    <!-- <div class="leaderboard-top flex flex-grow p-1 m-1 mt-2 mb-2 border-b border-gray-200 text-gray-200">
      <a href="#" class="rank" >Rank</a>|
      <a href="#" class="name" >Name</a>|
      <a href="#" class="points" >Points</a>
    </div> -->
    <p class="lg:text-5xl sm:text-4xl text-3xl mb-12"><i class="fas fa-chart-line "></i> Leaderboard</p>
    <leaderboard-lead name="Shetakawat Mourya" pid="234" rank="1" points="910"></leaderboard-lead>
    <leaderboard-item name="Abhishek sharma" pid="122" rank="2" points="900" class=""></leaderboard-item>
    <leaderboard-item name="Tushar Kapoor" pid="122" rank="3" points="876" class=""></leaderboard-item>
    <leaderboard-item name="Tanya Singh" pid="122" rank="4" points="873" class=""></leaderboard-item>
    <leaderboard-item name="Anurag Bhatia" pid="122" rank="5" points="800" class=""></leaderboard-item>
    <leaderboard-item name="Motit Singh" pid="122" rank="6" points="790" class=""></leaderboard-item>
    <leaderboard-item name="Prince Awana" pid="122" rank="23" points="544" class=""></leaderboard-item>
    <leaderboard-item name="Irshad" pid="122" rank="234" points="230" class=""></leaderboard-item>
    <leaderboard-item name="Abhishek sharma" pid="122" rank="2" points="900" class=""></leaderboard-item>
    <leaderboard-item name="Tushar Kapoor" pid="122" rank="3" points="876" class=""></leaderboard-item>
    <leaderboard-item name="Tanya Singh" pid="122" rank="4" points="873" class=""></leaderboard-item>
    <leaderboard-item name="Anurag Bhatia" pid="122" rank="5" points="800" class=""></leaderboard-item>
    <leaderboard-item name="Motit Singh" pid="122" rank="6" points="790" class=""></leaderboard-item>
    <leaderboard-item name="Prince Awana" pid="122" rank="23" points="544" class=""></leaderboard-item>
    <leaderboard-item name="Irshad" pid="122" rank="234" points="230" class=""></leaderboard-item>
  </div>
</template>

<style lang="css" scoped>
  .leaderboard{
    font-family: 'Bowlby One SC', cursive;
  }
  .name{
    flex:7
  }
  .id {
    flex : 1
  }
  .points{
    flex:2
  }
  .rank{
    flex:2
  }
</style>

<script>
import leaderboardItem from '@/components/leaderboardItem.vue'
import leaderboardLead from '@/components/leaderboardLead.vue'
export default {
  components : {
    'leaderboard-item' : leaderboardItem,
    'leaderboard-lead' : leaderboardLead
  }
}
</script>
