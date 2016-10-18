<style scoped>

</style>
<template>
    <div v-bind:id="id" class="tab" v-bind:class="status">
        <slot></slot>
    </div>
</template>
<script>
    module.exports = {
        props: {
            id:'',
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
