<script>
export default{
    name: "CompComics",
    props: {
        propsThumb: String,
        propsType: String,
    }
}
</script>

<!-- ----------------------------------------------------------------------------- -->

<template>

    <div>
        <figure>
            <img :src="propsThumb" alt="titolo">
        </figure>
    </div>
    <h3>{{propsType}}</h3>

</template>

<!-- ----------------------------------------------------------------------------- -->

<style lang="scss" scoped>

</style>
