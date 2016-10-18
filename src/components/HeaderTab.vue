<style scoped>
.bar, h1{
    color:#0a8ddf;
}
</style>
<template>
    <div class="bar bar-nav">
        <h1 class='title' v-text="title"></h1>
        <span class="icon" v-bind:class="iconClass"></span>
    </div>
</template>
<script>
    module.exports = {
        props: {
            title:'',
            icon:''
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

        },
        computed: {
            iconClass () {
                return "icon-"+this.icon
            }
        }
    }
</script>
