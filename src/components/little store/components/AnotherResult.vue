<template>
    <div>
        <p>Counter is: {{counter }}</p>
        <p> {{ str }}</p>
    </div>
</template>

<script>
    import {mapGetters} from 'vuex'

    export default {
        computed: {
            ...mapGetters({
                counter: 'doubleCounter',
                str: 'stringCounter'
            })
        }
    }
</script>
