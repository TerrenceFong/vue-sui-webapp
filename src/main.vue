<style>
    @import './assets/css/sm.css';
    .fade-transition {
        transition: opacity .3s ease;
    }
    .fade-enter, .fade-leave {
        opacity: 0;
    }
</style>

<template>
    <div class="page">
        <bar v-if="isIndex" class="bar bar-tab">
            <bar-item path="/home" label="首页" icon="home"></bar-item>
            <bar-item path="/search" label="发现" icon="search"></bar-item>
            <bar-item path="/message" label="消息" icon="message"></bar-item>
            <bar-item path="/me" label="我" icon="me"></bar-item>
        </bar>
        <router-view keep-alive transition-mode="out-in" transition="fade" ></router-view>
    </div>
</template>

<script>
import Bar from './components/Bar';
import BarItem from './components/BarItem';


module.exports = {
    components: {
        'bar':Bar,
        'bar-item':BarItem
    },
    data () {
        return {
            isIndex: true,
        }
    },
}
</script>