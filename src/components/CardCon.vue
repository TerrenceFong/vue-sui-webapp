<style scoped>

</style>
<template>
    <div class="card" v-on:click="goDetail">
        <slot></slot>
    </div>
</template>
<script>
    module.exports = {
        props: {
            
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
            goDetail: function(){
                this.$dispatch('GoDetailRouter', $(this.$el).index())
            }
        }
    }
</script>
