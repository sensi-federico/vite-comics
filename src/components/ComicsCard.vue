<script>
export default {
    name: 'ComicsCard',
    props: {
        url: String,
        title: String
    }
}
</script>
<template>
    <div class="col-2">
        <img :src="url" alt="">
        <p>{{ title }}</p>
    </div>
</template>