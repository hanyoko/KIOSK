<script>
    const products = {
        meatPasta01: {
            description:
            'Bacon and egg yolk with spaghetti in a cream sauce. Bacon and egg yolk with spaghetti in a cream sauce. Bacon and egg yolk with spaghetti in a cream sauce.',
            id: 'meatPasta01',
            name: 'Carbonara',
            picture: 'https://picsum.photos/300/200.webp',
            price: 1700,
        },
        meatPasta02: {
            description: '',
            id: 'meatPasta02',
            name: 'Bolognese',
            picture: 'https://picsum.photos/300/200.webp',
            price: 1700,
        },
        meatPasta03: {
            description: '',
            id: 'meatPasta03',
            name: 'Polpettine',
            picture: 'https://picsum.photos/300/200.webp',
            price: 1700,
        },
        meatPasta04: {
            description: 'Bacon and egg yolk with spaghetti in a cream sauce.',
            id: 'meatPasta04',
            name: 'Salscicie',
            picture: 'https://picsum.photos/300/200.webp',
            price: 1700,
        },
        meatPasta05: {
            description: '',
            id: 'meatPasta05',
            name: 'Rose Forno',
            picture: 'https://picsum.photos/300/200.webp',
            price: 1900,
        },
        meatPasta06: {
            description: '',
            id: 'meatPasta06',
            name: 'Beef Soy Pasta',
            picture: 'https://picsum.photos/300/200.webp',
            price: 1750,
        },
        meatPasta07: {
            description: '',
            id: 'meatPasta07',
            name: 'Beef Rose Pasta',
            picture: 'https://picsum.photos/300/200.webp',
            price: 1800,
        },
        meatPasta08: {
            description: '',
            id: 'meatPasta08',
            name: 'Meat Lover',
            picture: 'https://picsum.photos/300/200.webp',
            price: 1850,
        },
    }
</script>

<section>
    <div id="main">
        <div id="tit">
            <a href="/"><p>←</p></a>
            <h1 class="title">Meat Pasta</h1>
            <h2 class="dot">·</h2>
            <h2 class="subtitle">Pasta and Fries</h2>
        </div>

        <div id="a">
            <div class="list">
                <img alt="" src="{products.meatPasta01.picture}" />
                <p class="name">{products.meatPasta01.name}</p>
                <p class="price">${(products.meatPasta01.price*0.01).toFixed(2)}</p>
            </div>
            <div class="list">
                <img alt="" src="{products.meatPasta02.picture}" /> 
                <p class="name">{products.meatPasta02.name}</p>
                <p class="price">${(products.meatPasta02.price*0.01).toFixed(2)}</p>
            </div>
            <div class="list">
                <img alt="" src="{products.meatPasta03.picture}" /> 
                <p class="name">{products.meatPasta03.name}</p>
                <p class="price">${(products.meatPasta03.price*0.01).toFixed(2)}</p>
            </div>
        </div>
        <div id="b">
            <div class="list">
                <img alt="" src="{products.meatPasta04.picture}" /> 
                <p class="name">{products.meatPasta04.name}</p>
                <p class="price">${(products.meatPasta04.price*0.01).toFixed(2)}</p>
            </div>
            <div class="list">
                <img alt="" src="{products.meatPasta05.picture}" /> 
                <p class="name">{products.meatPasta05.name}</p>
                <p class="price">${(products.meatPasta05.price*0.01).toFixed(2)}</p>
            </div>
            <div class="list">
                <img alt="" src="{products.meatPasta06.picture}" /> 
                <p class="name">{products.meatPasta06.name}</p>
                <p class="price">${(products.meatPasta06.price*0.01).toFixed(2)}</p>
            </div>
        </div>
        <div id="c">
            <div class="list">
                <img alt="" src="{products.meatPasta07.picture}" /> 
                <p class="name">{products.meatPasta07.name}</p>
                <p class="price">${(products.meatPasta07.price*0.01).toFixed(2)}</p>
            </div>
            <div class="list">
                <img alt="" src="{products.meatPasta08.picture}" /> 
                <p class="name">{products.meatPasta08.name}</p>
                <p class="price">${(products.meatPasta08.price*0.01).toFixed(2)}</p>
            </div>
            <div class="list blank">
            </div>
        </div>
    </div>
</section>

<style>
    * { margin: 0; padding: 0; box-sizing: border-box; font-family: sans-serif, "맑은고딕"; } 
    a { text-decoration: none; color:inherit; }
    img { vertical-align: middle; border: none; }
    h1, h2 { font-weight: normal; }
    
    #tit {
        display: flex;
        text-align: center;
        align-items: center;
        margin-bottom: 30px;
        margin-left: 30px;
    }
    #tit a {
        width: 80px;
        height: 50px;
        font-size: 30px;
        font-weight: bold;
        text-align: center;
        align-items: center;
        border-radius: 5px;
        box-shadow: 2px 2px 2px 2px rgb(228, 226, 226);
    }
    #tit .title {
        font-size: 40px;
        font-weight: bold;
        padding: 0 30px;
    }
    #tit .dot {
        padding-right: 30px;
        font-weight: 500;
        color: gray;
    }
    #tit .subtitle {
        font-weight: 500;
        color: gray;
    }

    #main {
        width: 100%;
        height: 100vh;
        padding: 30px;
        display: flex;
        flex-direction: column;
    }
    #a, #b, #c {
        width: 100%;
        display: flex;
        justify-content: space-around;
    }
    .list {
        display: flex;
        flex-direction: column;
        text-align: center;
        align-items: center;
        width: 29%;
        height: 400px;
        margin-bottom: 100px;
    }
    .list img {
        width: 100%;
        height: 350px !important;
        border-radius: 10px;
        object-fit: fill;
    }
    .list p {
        font-size: 30px;
        padding: 10px 0;
        margin-top: 3px;
    }
    .list .price {
        color: gray;
    }

    @media screen and (max-width:1199px) {
    /* 테블릿 가로 */
        .list {
            margin-bottom: 40px;
        }
    }

    @media screen and (max-width:899px) {
    /* 모바일 가로, 테블릿 세로 */
        .list img {
            height: 400px !important;
        }

        #tit {
            margin-left: 0;
        }
        #tit .title {
            font-size: 2rem;
            font-weight: bold;
            padding: 0 1rem;
        }
        #tit .dot {
            padding-right: 1rem;
            font-weight: 500;
            color: gray;
        }
        #tit .subtitle {
            font-weight: 500;
            color: gray;
        }
    }

    @media screen and (max-width:599px) {
    /* 모바일 세로 */
        #a, #b, #c {
            flex-direction: column;
        }
        .list {
            width: 100%;
            height: 400px !important;
            margin-bottom: 80px;
        }
        .list .name {
            font-weight: bold;
        }
        #tit a {
            width: 70px;
            font-size: 2rem;
        }
        #tit .title {
            font-size: 2rem;
            font-weight: bold;
            padding: 0 1.8rem;
        }
        #tit .dot {
            font-size: 0;
        }
        #tit .subtitle {
            font-size: 0;
        }

        .blank {
            display: none;
        }
    }
</style>