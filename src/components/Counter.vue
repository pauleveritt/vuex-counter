<template>
    <div>
        <p>Clicked {{ count }} times! Count is {{ parity }}.</p>
        <button @click="increment">Increment</button>
        <button @click="decrement">Decrement</button>
    </div>

</template>

<script>
    import {mapState, mapGetters, mapActions} from 'vuex'

    export default {
        name: 'Counter',
        computed: {
            ...mapState([
                'count'
            ]),
            ...mapGetters([
                'parity'
            ])
        },
        methods: mapActions([
            'increment',
            'decrement'
        ])
    }
</script>
