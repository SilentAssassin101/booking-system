<template>
    <div class="card w-96 bg-base-100 shadow-xl image-full">
        <figure><img :src="imgSrc" :alt="description" /></figure>
        <div class="card-body">
            <h2 class="card-title">{{ title }}</h2>
            <p>{{ description }}</p>
            <div class="card-actions justify-end">
                <button class="btn btn-primary"><a :href="buttonTarget" target="_blank">{{ buttonText }}</a></button>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'CardOverlay',
    components: {
    },
    props: {
        imgSrc: {
            type: String,
            default: 'https://daisyui.com/images/stock/photo-1606107557195-0e29a4b5b4aa.jpg'
        },
        title: {
            type: String,
            default: 'Shoes!'
        },
        description: {
            type: String,
            default: 'If a dog chews shoes whose shoes does he choose?'
        },
        buttonText: {
            type: String,
            default: 'Buy Now'
        },
        buttonTarget: {
            type: String,
            default: '#'
        }
    }
}
</script>

<style></style>