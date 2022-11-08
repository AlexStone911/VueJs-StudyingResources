<template>
    <ul>
        <resource-item v-for="res in resources"
                       :key="res.id"
                       :title="res.title"
                       :link="res.link"
                       :desc="res.description">
        </resource-item>
    </ul>l
</template>

<script>
import ResourceItem from './ResourceItem.vue';

export default {
    components: {
        ResourceItem
    },
    inject: ['resources']
}
</script>

<style scoped>
ul {
    list-style: none;
    margin: 0;
    padding: 0;
    margin: auto;
    max-width: 40rem;
}
</style>