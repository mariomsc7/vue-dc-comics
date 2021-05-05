<template>
    <div class="box">
        <div class="images">
            <img :src="details.thumb" :alt="details.type">
            <h4> {{ details.series }} </h4>
        </div>

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

    .box {
        margin: 30px 0;
    }

    .images {
        max-width: 200px;
    }

    .images img {
        width: 200px;
        height: 200px;
        cursor: pointer;
    }

    .images h4 {
        margin-top: 20px;
        color: #fff;
        text-align: center;
        letter-spacing: 2px;
        cursor: pointer;
    }

    

</style>