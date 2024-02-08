<script>
export default{
    name: "CompComics",
    props: {
        propsThumb: String,
        propsSeries: String,
    }
}
</script>

<!-- ----------------------------------------------------------------------------- -->

<template>

    <div class="serie">
        <figure>
            <img :src="propsThumb" alt="titolo">
        </figure>
        <p>{{propsSeries}}</p>
    </div>

</template>

<!-- ----------------------------------------------------------------------------- -->

<style lang="scss" scoped>
.serie{
    flex-basis: calc(100% / 6);
    color: white;
    padding: 10px;
    p{
        margin: 10px 0;
    }
    figure{
        height: 200px;
        img{
            width: 100%;
            height: 100%;
            display: block;
        }
    }
}
</style>
