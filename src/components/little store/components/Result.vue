<template>
    <div>
        <p>Counter is: {{ counter }}</p>
        <p> {{ str }}</p>
        <p>$store.state.counter => {{$store.state.counter}} </p>
    </div>
</template>

<script>
    export default {

        computed: {
            counter() {
                return this.$store.getters.doubleCounter;
            },
            str(){
                return this.$store.getters.stringCounter;

            }

        }
    }
</script>