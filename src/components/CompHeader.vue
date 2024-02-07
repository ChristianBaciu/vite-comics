<script>
export default{
    name: "CompHeader"
}
</script>


<!-- ----------------------------------------------------------------------------- -->



<template>

    <header>
        <figure>
            <img src="../assets/img/dc-logo.png" alt="">
        </figure>

        <div>
            <ul>
                <li><a href="#"></a>character</li>
                <li><a href="#"></a>comics</li>
                <li><a href="#"></a>movies</li>
                <li><a href="#"></a>tv</li>
                <li><a href="#"></a>games</li>
                <li><a href="#"></a>collectibles</li>
                <li><a href="#"></a>videos</li>
                <li><a href="#"></a>fans</li>
                <li><a href="#"></a>news</li>
                <li><a href="#"></a>shop</li>
            </ul>
        </div>
    </header>
    <main>
        <p>--&gt; Content goes here &lt;--</p>
    </main>


</template>


<!-- ----------------------------------------------------------------------------- -->


<style lang="scss" scoped>

header{
    background-color: white;
    display: flex;
    ul{
        li{
            color: red;
        }
    }
}
p{
    background-color: #1c1c1c;
    padding: 50px;
    color: white;
}
</style>
