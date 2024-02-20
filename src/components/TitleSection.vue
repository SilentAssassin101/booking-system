<template>
    <div
        class="p-2 m-8 text-center max-w-96 mx-auto border-2 border-primary rounded-box bg-gradient-to-br from-base-300 to-primary/20">
        <h2 class="text-4xl font-bold">{{ title }}</h2>
        <p class="py-5 text-lg">{{ description }}</p>
    </div>
</template>

<script>
export default {
    name: 'TitleSection',
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