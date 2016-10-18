<style scoped>

</style>
<template>
<div class="hello">
    <h1>{{ msg }}</h1>
</div>
</template>
<script>
    module.exports = {
        data () {
            return {
                msg: 'search!'
            }
        },
        ready () {
            $.init();
        },
        beforeDestroy () {

        },
        methods: {
            
        }
    }
</script>
