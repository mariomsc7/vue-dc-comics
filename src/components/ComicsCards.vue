<template>
    <div class="box">
        <img :src="details.thumb" :alt="details.type">
        <h2> {{ details.series }} </h2>
    </div>
</template>

<script>
export default {
    name : 'ComicsCards',
    props: ['details'],
    // props : {
    //        details : Object
    // }
}
</script>

<style scoped>


    .box img {
        width: 200px;
        height: 200px;
    }
</style>