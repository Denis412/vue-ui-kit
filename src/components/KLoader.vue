<template>
    <div class="k-loader" :style="styles">
        <div></div>
        <div></div>
        <div></div>
        <div></div>
    </div>
</template>

<script>
import { computed } from 'vue';
export default {
    name: 'KLoader',
    props: {
        size: {
            type: String,
            default: 'md',
        },
        color: {
            type: String,
            default: '#fff',
        },
    },
    setup(props) {
        const styles = computed(() => {
            return {
                '--size-k-loader': `var(--size-${props.size})`,
                '--color-k-loader': props.color,
            };
        });

        return {
            styles,
        };
    },
};
</script>

<style lang="scss" scoped></style>
