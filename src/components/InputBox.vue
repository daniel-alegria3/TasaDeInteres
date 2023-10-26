<script setup>
    // import { ref } from 'vue'
    defineProps({
        label: {
            type: String,
            required: true,
        },
        type: {
            type: String,
            required: false,
        },
        value: {
            type: String,
            required: false,
        },
        name: {
            type: String,
            required: false,
        },
    })
    // defineProps([
    //     "label", "type"
    // ])
</script>

<template>
    <div class="idk">
        <label>
            {{ label }}
            <input :type="type" :value="value" :name="name"/>
        </label>
    </div>
</template>

<style scoped>
</style>

