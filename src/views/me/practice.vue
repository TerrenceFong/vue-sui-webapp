<style scoped>
.me-container{
    padding-top:2.2rem;
}
</style>
<template>
    <div>
        <me-header-tab title="最佳实现" router="/me"></me-header-tab>
        <div class="me-container">
            {{msg}}
        </div>
    </div>
</template>
<script>
    import MeHeaderTab from '../me/MeHeaderTab.vue';

    module.exports = {
        components:{
            'me-header-tab': MeHeaderTab
        },
        data () {
            return {
                msg:'这里应该有些最佳实现'
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