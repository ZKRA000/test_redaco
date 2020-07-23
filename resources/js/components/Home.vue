<template>

    <div class="container" :class="{bodyNight:night,bodyLight:light}">

        <div class="navbar" :class="{BackgroundNight:night,BackgroundLight:light}">
            <div :class="{TextNight:night,TextLight:light}">
                Redaco
            </div>

            <div class="bars">
                <div :class="{BarsNight:night,BarsLight:light}"></div>
                <div :class="{BarsNight:night,BarsLight:light}"></div>
                <div :class="{BarsNight:night,BarsLight:light}"></div>
            </div>
        </div>

        <div class="header" :class="{TextNight:night,TextLight:light}">
            We are Redaco, Hello Dribbble.
        </div>

        <div class="image-landing" :class="{personNight:night,personLight:light}">
            <img src="/images/image-navy.svg" />
        </div>

        <div class="img-dribbble" v-on:click="switchTheme()">
            <img src="/images/button dribbble.png" />
        </div>

    </div>

</template>

<script>
    export default {
        data: function () {
            return {
                night: true,
                light: false
            }
        },
        methods: {
            switchTheme: function () {
                this.night = !this.night;
                this.light = !this.light;
            }
        }
    }

</script>

<style lang="sass">

</style>
