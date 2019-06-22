<template>
    <div>
        <p>Counter is: {{ doubleCounter }}</p>
        <p>Number of click: {{ stringCounter }}</p>
    </div>
</template>

<script>
    import {mapGetters }  from 'vuex';
    export default {
        computed: {
            ...mapGetters([
                'doubleCounter',
                'stringCounter'
            ])
        }
        // computed: mapGetters([
        //     'doubleCounter',
        //     'stringCounter'
        // ])
        // computed: {
        //     counter() {
        //         return  this.$store.getters.doubleCounter;
        //     },
        //     clicks() {
        //         return  this.$store.getters.;
        //     }
        // }
    }
</script>