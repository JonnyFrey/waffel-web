<template>
    <div>
        <Slide id="nav" width="100">
            <home-menu-item title="Home" iconType="home" link="/"/>
            <home-menu-item title="About" iconType="info-circle" link="/about"/>
        </Slide>
    </div>
</template>

<script>
    import { Slide } from 'vue-burger-menu';
    import HomeMenuItem from '@/components/HomeMenuItem.vue';

    export default {
        components: {
            Slide,
            HomeMenuItem,
        },
    };
</script>

<style>
    #nav {
        padding: 30px;
    }

    #nav .bm-menu {
        background: #1c1c1c;
    }

    #nav .bm-burger-bars {
        background: limegreen;
    }
    
    #nav .icon-name {
        padding-left: 10%;
        padding-top: 1%;
    }

    #nav .bm-cross-button {
        height: 33px;
        width: 33px;
        left: 35%;
        top: 3%;
    }

</style>
