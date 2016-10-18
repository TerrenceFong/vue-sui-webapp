<style scoped>

</style>
<template>
    <div :class="classType">
        <slot></slot>
    </div>
</template>
<script>
    module.exports = {
        props: {
            type:''
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
        computed:{
            classType: function(){
                return 'card-'+this.type
            }
        }
    }
</script>
