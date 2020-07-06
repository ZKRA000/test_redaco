<template>
    
    <div class="container" v-bind:class="{bodyNight:night,bodyLight:light}">
       <div class="navbar" v-bind:class="{BackgroundNight:night,BackgroundLight:light}">
          <div v-bind:class="{TextNight:night,TextLight:light}">
           Redaco
          </div>
          <div class="bars" >
            <div v-bind:class="{BarsNight:night,BarsLight:light}"></div>
            <div v-bind:class="{BarsNight:night,BarsLight:light}"></div>
            <div v-bind:class="{BarsNight:night,BarsLight:light}"></div>
          </div>
        </div>
      <div class="header" v-bind:class="{TextNight:night,TextLight:light}">
        We are Redaco, Hello Dribbble.
      </div>
      <div class="image-landing" v-bind:class="{personNight:night,personLight:light}">
            <img src="/images/image-navy.svg"/>
      </div>
      <div class="img-dribbble" v-on:click="switchTheme()">
           <img src="/images/button dribbble.png"/>
      </div>
      
    </div>
</template>

<script>
    export default {
        data:function(){
            return {
              night: true,
              light: false
            }
        },
        methods:{
            switchTheme : function(){
                this.night = !this.night;
                this.light = !this.light;
            }
        }
    }
</script>

<style lang="sass">
  @import "../../sass/main.scss"
</style>

