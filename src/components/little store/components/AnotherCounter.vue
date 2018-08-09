<template>
    <div style="border: medium solid red">
        <p>Another counter</p>
        <button class="btn btn-primary" @click="increment({by:50,dur:500})">Asyc Increment </button>
        <button class="btn btn-primary" @click="decrement(50)">Decrement</button>
    </div>
</template>
<script>
    // import {mapMutations} from 'vuex';
     import {mapActions} from 'vuex';

    export default {
        methods: {
//            ...mapMutations([
//                'increment',
//                'decrement'
//            ]),
            ...mapActions([
                'increment',
                'decrement'
            ])
        }
    }
</script>