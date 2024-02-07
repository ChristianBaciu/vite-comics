<script>
export default{
    name: "CompHeader",
    data(){
        return{
            ArrayLinksMenu:[
                {
                    nome: 'CHARACTER',
                    link: '#',
                    valore: 'false'
                },
                {
                    nome: 'COMICS',
                    link: '#',
                    valore: 'true',
                },
                {
                    nome: 'MOVIES',
                    link: '#',
                    valore: 'false',
                },
                {
                    nome: 'TV',
                    link: '#',
                    valore: 'false',
                },
                {
                    nome: 'GAMES',
                    link: '#',
                    valore: 'false',
                },
                {
                    nome: 'COLLECTIBLES',
                    link: '#',
                    valore: 'false',
                },
                {
                    nome: 'VIDEOS',
                    link: '#',
                    valore: 'false',
                },
                {
                    nome: 'FANS',
                    link: '#',
                    valore: 'false',
                },
                {
                    nome: 'NEWS',
                    link: '#',
                    valore: 'false',
                },
                {
                    nome: 'SHOP',
                    link: '#',
                    valore: 'shop',
                },
            ]
        }
    }
}
</script>

<!-- ----------------------------------------------------------------------------- -->

<template>

    <header>
        <figure>
            <img src="../assets/img/dc-logo.png" width="80" alt="logo">
        </figure>

        <nav>
            <ul>
                <li v-for="(element,index) in ArrayLinksMenu" :key="index">
                    <a :href="element.index">{{ element.nome }}</a>
                </li>
            </ul>
        </nav>

    </header>
    <main>
        <h2>--&gt; Content goes here &lt;--</h2>
    </main>


</template>

<!-- ----------------------------------------------------------------------------- -->

<style lang="scss" scoped>

header{
    height: 15vh;
    display: flex;
    display: flex;
        align-items: center;
        justify-content: space-between;
        width: 80%;
        margin: 0 auto;

    ul{
        display: flex;
        align-items: center;
        gap: 20px;
        li{
            display: flex;
            list-style-type: none;
            color: #3b383a;
        }
    }
}
main{
    background-color: #1c1c1c;
    height: 15vh;
    display: flex;
    align-items: center;
    h2{
        color: white;
        width: 80%;
        margin: 0 auto;
    }
}
</style>
