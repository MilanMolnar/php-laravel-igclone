<template>
    <div v-on:mousemove="init">
        <a style="text-decoration: none; color: white"  href="/cctv">CCTV  ►►</a>
    </div>
</template>


<script>
    import VanillaTilt from 'vanilla-tilt';

    export default {
        mounted() {
            console.log('Component mounted.')
        },
        data: function () {
            return {
            }
        },
        methods: {
            init(){
                VanillaTilt.init(document.querySelector('#cctv-btn'))
            }
        }
    }
</script>

