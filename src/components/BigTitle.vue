<template>
    <div class="title_text">
        {{ leftMessage }}<span class="left_title">{{ leftMessageColor }}</span><span class="right_title">{{ rightMessageColor }}</span>{{ rightMessage }}
    </div>
</template>

<script lang="ts">
    import {Component, Prop, Vue} from 'vue-property-decorator';

    @Component
    export default class BigTitle extends Vue {
        @Prop() private leftMessage!: string;
        @Prop() private rightMessage!: string;
        @Prop() private leftMessageColor!: string;
        @Prop() private rightMessageColor!: string;
    }

</script>

<style scoped>

    .title_text {
        color: white;
        font-size: 6vw;
        font-family: "Courier New", serif;
        position: absolute;
        top: 50%;
        left: 50%;
        -moz-transform: translateX(-50%) translateY(-50%);
        -webkit-transform: translateX(-50%) translateY(-50%);
        transform: translateX(-50%) translateY(-50%);
        margin: 0 -50% 0 0;
    }

    .title_text .left_title {
        color: hotpink;
    }

    .title_text .right_title {
        color: limegreen;
    }

</style>
