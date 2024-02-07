<script>
export default{
    name: "CompMain",
    data(){
        return{
            ArrayLinksMenu:[
                {
                    nome: 'Character',
                    link: '#',
                    valore: 'false'
                },
                {
                    nome: 'Comics',
                    link: '#',
                    valore: '',
                },
                {
                    nome: 'Movies',
                    link: '#',
                    valore: 'false',
                },
                {
                    nome: 'Tv',
                    link: '#',
                    valore: 'false',
                },
                {
                    nome: 'Games',
                    link: '#',
                    valore: 'false',
                },
            ]
        }
    }

}
</script>


<!-- ----------------------------------------------------------------------------- -->



<template>

        <header>
            <ul>
                <li v-for="(element,index) in ArrayLinksMenu" :key="index">
                    <a :href="element.index">{{ element.nome }}</a>
                </li>
            </ul>
        </header>

        <main>
            <div>
                <h3>dc comics</h3>
            </div>

        </main>

        <!-- <footer>

        </footer> -->

</template>


<!-- ----------------------------------------------------------------------------- -->


<style lang="scss" scoped>
header{
    background-color: #0282f9;
    height: 15vh;
    display: flex;
    justify-content: space-around;
    align-items: center;
    ul{
        color: white;
        display: flex;
        gap: 60px;
        li{
            list-style-type: none;
        }
    }
}
main{
    background-color: orange;
    height: 40vh;
}
// footer{
//     height: 15vh;
//     background-color: #303030;
// }
</style>
