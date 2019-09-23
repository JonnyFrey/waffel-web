<template>
    <div class="menu-item">
        <router-link :to="link">
            <b-icon
                    pack="fas"
                    :icon="iconType"
                    size="is-medium"
                    type="is-info">
            </b-icon>
            {{ title }}
        </router-link>
    </div>
</template>

<script lang="ts">

    import Component from 'vue-class-component';
    import {Prop, Vue} from 'vue-property-decorator';

    @Component
    export default class HomeMenuItem extends Vue {
        @Prop() private link!: string;
        @Prop() private iconType!: string;
        @Prop() private title!: string;
    }

</script>

<style>

    .menu-item a.router-link-exact-active {
        color: #42b983;
    }

    .menu-item a {
        font-weight: bold;
        color: #ac4779;
        padding-right: 20px;
    }

</style>
