<style scoped>
h3{
    text-align: center;
}
p{
    background: #fff;
    padding: 2rem 0.5rem;
    margin: 0;
}
.me-container{
    padding-top:2.2rem;
}
</style>
<template>
    <div>
        <me-header-tab title="详细页" router="/首页"></me-header-tab>
        <div class="me-container">
            <!-- <h3>详情页</h3> -->
            <p>{{Lcontent}}</p>
        </div>
    </div>
</template>
<script>
    import MeHeaderTab from './me/MeHeaderTab.vue';

    module.exports = {
        components:{
            'me-header-tab': MeHeaderTab
        },
        route: {
            data: function(transition){
                this.$set('Lcontent',decodeURIComponent(this.$route.params.Lcontent)); 
            }
        },
        data () {
            return {
                Lcontent : ''
            }
        },
        ready () {
            $.init()
        },
        beforeDestroy () {

        },
        methods: {
            
        }
    }
</script>