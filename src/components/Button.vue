<style scoped>

</style>
<template>
    <a :href="path" class="tab-link button" v-bind:class="status" v-text="label"></a>
</template>
<script>
    module.exports = {
        props: {
            path:'',
            label:'',
            status:''
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
