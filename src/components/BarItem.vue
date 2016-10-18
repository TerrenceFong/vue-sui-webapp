<style scoped>

</style>
<template>
<a class="tab-item external" v-link="{ path: path, activeClass: 'active', replace: true }">
    <span class="icon" :class="iconClass"></span>
    <span class="tab-label" v-text="label"></span>
</a>
</template>
<script>
    module.exports = {
        props: {
            label:'',
            path:'',
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
            iconClass(){
                return "icon-"+this.icon
            }
        }
    }
</script>
