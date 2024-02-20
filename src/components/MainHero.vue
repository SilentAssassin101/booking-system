<template>
    <div class="hero min-h-screen bg-base-200">
        <div class="hero-content text-center">
            <div class="max-w-md">
                <h1 class="text-5xl font-bold">{{ title }}</h1>
                <p class="py-6">{{ description }}</p>
                <button class="btn btn-primary"><a :href="buttonTarget">{{ buttonText }}</a></button>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'MainHero',
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
        buttonText: {
            type: String,
            default: 'Get Started'
        },
        buttonTarget: {
            type: String,
            default: '#'
        }
    }
}
</script>

<style></style>