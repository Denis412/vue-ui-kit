<template>
    <div class="container">
        <k-loader />
    </div>
</template>

<script>
import KLoader from './components/KLoader.vue';

export default {
    name: 'App',
    components: {
        KLoader,
    },
};
</script>

<style lang="scss">
.container {
    background-color: lightblue;
    padding: 24px;
}
</style>
