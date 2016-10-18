<style scoped>
.img-area{
    width: 100%;
}
.img-area img{
    width: 100%;
    display: block;
}
.row .col-50{
    padding: 0.9rem 0;
    height: 4rem;
}
.grid-demo{
    position: relative;
}
.bar-nav~.content {
    top: 17rem;
    bottom: 3rem;
}
.col-50{
    background: #fff;
    margin-bottom: 0.5rem;
    text-align: center;
}
.tab-item{
    display: block;
}
.tab-label{
    color: #555;
    font-family: '黑体';
    font-size: 0.8rem;
}

</style>

<template>
<div class="content">
    <div class="content-padded grid-demo">
        <div class="row">
            <div v-for="(index, list) in lists" class="col-50">
                <a class="tab-item" v-link="{ path: list.path }">
                    <!-- 这里不同于首页的tab标签切换，所以不需要replace这个参数，让路由可以后退 -->
                    <span class="icon" v-bind:class="list.icon"></span>
                    <br>
                    <span class="tab-label">{{list.title}}</span>
                </a>
            </div>
        </div>
    </div>
</div>
</template>

<script>
    import $ from 'zepto';
    module.exports = {
        props: {
            lists:'',
            icon:'',
        },
        data () {
            return {

            }
        },
        ready () {
            $.init();
        },
        beforeDestroy () {

        },
        methods: {

        },
        computed: {
            iconClass: function(){
                return "icon-"+this.icon
            }
        }
    }
</script>
