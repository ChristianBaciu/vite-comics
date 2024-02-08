<script>
export default{
    name: "CompHeader",
    data(){
        return{
            ArrayHeaderMenu:[
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
                <li v-for="(element,index) in ArrayHeaderMenu" :key="index">
                    <a :href="element.index">{{ element.nome }}</a>
                </li>
            </ul>
        </nav>
    </header>




    <main>


    </main>


</template>

<!-- ----------------------------------------------------------------------------- -->

<style lang="scss" scoped>

header{
    background-color: white;
    height: 15vh;
    display: flex;
    align-items: center;
    justify-content: space-around;

    ul{
        display: flex;
        align-items: center;
        gap: 20px;
        li{
            display: flex;
            list-style-type: none;
            font-weight: bolder;
            &:hover{
            color: red;
        }

        }
    }
}
main{
    background-image: url('../assets/img/jumbotron.jpg');
    background-repeat: no-repeat;
    background-position: top;
    background-size: cover;
    height: 45vh;
    display: flex;
    align-items: center;
}
</style>
