<script>
export default{
    name: "CompMain",
    data(){
        return{
            ArrayBlueMenu:[
                {
                    nome: 'DIGITAL COMICS',
                    img: 'buy-comics-digital-comics.png',
                },
                {
                    nome: 'DC MERCHANDISE',
                    img: 'buy-comics-merchandise.png',
                },
                {
                    nome: 'SUBSCRIPTION',
                    img: 'buy-comics-subscriptions.png',
                },
                {
                    nome: 'COMIC SHOP LOCATOR',
                    img: 'buy-comics-shop-locator.png',
                },
                {
                    nome: 'DC POWER VISA',
                    img: 'buy-dc-power-visa.png',
                },
            ],
        }
    }

}
</script>

<!-- ----------------------------------------------------------------------------- -->

<template>
    <header>
        <ul>
            <li v-for="(element, index) in ArrayBlueMenu" :key="index">
                <img :src="`./src/assets/img/${element.img}`" width="40" alt="comics">
                <p>{{ element.nome }}</p> 
            </li>
        </ul>
    </header>

    <main>
        <nav>
            <section>
                <div>
                    <h2>DC COMICS</h2>
                    <ul>
                        <li>Characters</li>
                        <li>Comics</li>
                        <li>Movies</li>
                        <li>TV</li>
                        <li>Games</li>
                        <li>Videos</li>
                        <li>News</li>
                    </ul>

                    <h2>SHOP</h2>
                    <ul>
                        <li>Shop DC</li>
                        <li>Shop DC Collectibles</li>
                    </ul>
                </div>

                <div>
                    <h2>DC</h2>
                    <ul>
                        <li>Terms Of Use</li>
                        <li>Privacy policy (New)</li>
                        <li>Ad Choices</li>
                        <li>Advertising</li>
                        <li>Jobs</li>
                        <li>Subscriptions</li>
                        <li>Talent Workshops</li>
                        <li>CPSC Certificates</li>
                        <li>Shop Help</li>
                        <li>Contact Us</li>
                    </ul>

                </div>

                <div>
                    <h2>SITES</h2>
                    <ul>
                        <li>DC</li>
                        <li>MAD Magazine</li>
                        <li>DC Kids</li>
                        <li>DC Universe</li>
                        <li>DC Power Visa</li>
                    </ul>
                </div>
            </section>
        </nav>
    </main>
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
            display: flex;
            align-items: center;
        }
    }
}

main{
    background-image: url('../assets/img/footer-bg.jpg');
    background-repeat: no-repeat;
    background-position: top;
    background-size: cover;
    height: 43vh;
    display: flex;
    justify-content: center;

    nav{
        width: 80%;
        display: flex;
        gap: 50px;
        justify-content: space-between;
        padding: 20px 0;
        background-image: url('../assets/img/dc-logo-bg.png');
        background-repeat: no-repeat;
        background-position: right;

        section{
            display: flex;
            gap: 40px;

            h2{
            color: white;
            padding: 10px 0;
            }

            ul{
                li{
                    color: #949595;
                    list-style-type: none;

                }
            }
        }
    }
}
</style>
