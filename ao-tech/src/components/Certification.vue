<script setup lang="ts">
import { ref } from 'vue'
import ExpandIcon from './icons/expand.vue'
import CollapseIcon from './icons/collapse.vue'
const expanded = ref(false);
</script>
<template>
    <div class="item">
        <div class="header-wrapper" @click="expanded = !expanded">
            <div class="header">
                <slot name="header"></slot>
            </div>
            <div class="where">
                <div v-if="expanded" class="expander"><CollapseIcon /></div>
                <div v-else class="expander"><ExpandIcon /></div>
            </div>
        </div>
        <div class="content-wrapper" v-if="expanded">
            <div class="where">
                <slot name="where"></slot>
            </div>
            <div class="when">
                <slot name="when"></slot>
            </div>
        </div>
    </div>
</template>
  
<style scoped lang="scss">
.item {
    margin-top: 2rem;
    display: flex;
    flex-direction: column;
    width: 100%;
    position: relative;
    color: #ddd;
    padding-bottom: 10px;

    .header-wrapper {
        display: flex;
        justify-content: space-between;

        .header {
            font-weight: 700;
            padding-right: 20px;
        }

        .where {
            font-weight: 200;
            display: flex;
            position: relative;
            left: -14px;
            .expander {
                padding-left: 10px;
                height: 20px;
                width: 20px;
            }
        }
    }
    .content-wrapper{
        background-color: #333333;
        padding: 0 10px;
    }
}

.details {

    flex: 1;
    margin-left: 1rem;
}

i {
    display: flex;
    place-items: center;
    place-content: center;
    width: 32px;
    height: 32px;

    color: var(--color-text);
}

h3 {
    font-size: 1.2rem;
    font-weight: 500;
    margin-bottom: 0.4rem;
    color: var(--color-heading);
}

@media (min-width: 1024px) {
    .item {
        margin-top: 0;
    }

    i {
        top: calc(50% - 25px);
        left: -26px;
        position: absolute;
        border: 1px solid var(--color-border);
        background: var(--color-background);
        border-radius: 8px;
        width: 50px;
        height: 50px;
    }

    .item:before {
        content: ' ';
        border-left: 1px solid var(--color-border);
        position: absolute;
        left: 0;
        bottom: calc(50% + 25px);
        height: calc(50% - 25px);
    }

    .item:after {
        content: ' ';
        border-left: 1px solid var(--color-border);
        position: absolute;
        left: 0;
        top: calc(50% + 25px);
        height: calc(50% - 25px);
    }

    .item:first-of-type:before {
        display: none;
    }

    .item:last-of-type:after {
        display: none;
    }
}</style>
  