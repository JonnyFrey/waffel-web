<template>
    <div class="error blink">
        <BigTitle left-message-color="404 " right-message-color="Not Found"/>
    </div>
</template>

<script lang="ts">

    import {Component, Vue} from 'vue-property-decorator';
    import BigTitle from '@/components/BigTitle.vue';

    @Component({
        components: {
            BigTitle,
        },
    })
    export default class NotFound extends Vue {}

</script>

<style scoped>
    .blink {
        animation: blinker 1s linear infinite;
        text-decoration: blink;
    }

    @keyframes blinker {
        50% { opacity: 0; }
    }

</style>
