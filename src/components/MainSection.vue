<template>
    <div class="p-2">
        <h2 class="text-3xl font-bold">{{ title }}</h2>
        <p class="py-6">{{ description }}</p>
    </div>
</template>

<script>
export default {
    name: 'MainSection',
    components: {
    },
    props: {
        title: {
            type: String,
            default: 'Civil Booking'
        },
        description: {
            type: String,
            default: 'Welcome to Civil Booking'
        },
    }
}
</script>

<style></style>