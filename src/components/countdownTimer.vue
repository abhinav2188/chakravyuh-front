<template>


      <div class="container timer mx-auto flex p-2 text-gray-400 text-sm">
        <div class="w-1/4 p-2">
          <p class="timer-el">{{days}}</p>
          <p>Days</p>
        </div>
        <div class="w-1/4 p-2" >
          <p class="timer-el" >{{hours}}</p>
          <p>Hours</p>
        </div>
        <div class="w-1/4 p-2">
          <p class="timer-el">{{minutes}}</p>
          <p>Minutes</p>
        </div>
        <div class="w-1/4 p-2">
          <p class="timer-el">{{seconds}}</p>
          <p>Seconds</p>
        </div>
    </div>


</template>

<style lang="css" scoped>

    .timer{
        display:flex;
        flex-direction:row;
        justify-content : center;
        width: 500px;

    }
    .timer-el{
        font-weight : 100;
        border : 2px dotted #454545;
        border-radius : 10px;
        width: 100%;
        height : 100px;
        margin-bottom : 0px;
        padding-top : 1rem;
        padding-bottom: 1rem;
        font-size : 2.5rem;
    }

</style>


<script>

    export default{

        data: function(){
            return{
                eventDate : new Date('2020','01','24'),
                currentDate : new Date(),
                seconds : 0,
                minutes : 0,
                hours : 0,
                days : 0
            }
        },

        computed:{
            remTime: function(){
                return this.eventDate.getTime() - this.currentDate.getTime();
            },

        },

        methods :{
            updateTimer : function(){
                var date = new Date();
                var r = this.eventDate.getTime() - date.getTime();
                var s = r/1000;
                var m = s/60;
                var h = m/60;
                this.days = Math.floor(h/24);
                h = Math.floor(h % 24);
                m = Math.floor(m % 60);
                s = Math.floor(s % 60);
                this.hours = h<10 ? '0'+h : h;
                this.minutes = m<10?'0'+m:m;
                this.seconds = s<10?'0'+s:s;

                var self = this;
                setTimeout(function(){
                    self.updateTimer();
                }, 1000);
            }
        },

        mounted: function(){
            this.updateTimer();
        },

    }

</script>
