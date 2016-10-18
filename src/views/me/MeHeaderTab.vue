<style scoped>

</style>
<template>
    <div class="bar bar-nav">
        <h1 class='title' v-text="title"></h1>
        <a class="icon icon-left" v-link="{path: router}"></a>
    </div>
</template>
<script>
    module.exports = {
        props: {
            title:'',
            router:''
        },
        data () {
            return {

            }
        },
        ready () {

        },
        beforeDestroy () {

        },
        methods: {

        }
    }
</script>
