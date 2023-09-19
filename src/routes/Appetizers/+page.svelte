<script>
    import defaultPic from '$lib/img/gray.jpg';

    const products = {
        appetizer01: {
            description: 'Romain lettuce and croutons with caesar dressing.',
            id: 'appetizer01',
            name: 'Caesar Salad',
            picture: 'https://picsum.photos/300/200.webp',
            price: 1000,
        },
        appetizer02: {
            description: 'Green Salad.',
            id: 'appetizer02',
            name: 'Green Salad',
            picture: 'https://picsum.photos/300/200.webp',
            price: 1000,
        },
        appetizer03: {
            description: 'Caprese Salad.',
            id: 'appetizer03',
            name: 'Caprese Salad',
            picture: 'https://picsum.photos/300/200.webp',
            price: 1300,
        },
        appetizer04: {
            description: '',
            id: 'appetizer04',
            name: 'Calamari',
            picture: 'https://picsum.photos/300/200.webp',
            price: 1200,
        },
        appetizer05: {
            description: '',
            id: 'appetizer05',
            name: 'French Fries',
            picture: 'https://picsum.photos/300/200.webp',
            price: 800,
        },
        appetizer06: {
            description: '',
            id: 'appetizer06',
            name: 'Cheese Stick',
            price: 700,
        },
    }

</script>

<section>
    <div id="main">
        <div id="nav2">
            <a href="/"><p>←</p></a>
            <h1 class="title">Appetizer</h1>
            <h2 class="dot">·</h2>
            <h2 class="subtitle">Salad and Fries</h2>
        </div>

        <div id="a">
            <div class="list">
                <img alt="" src="{products.appetizer01.picture}" />
                <p class="name">{products.appetizer01.name}</p>
                <p class="price">${(products.appetizer01.price*0.01).toFixed(2)}</p>
            </div>
            <div class="list">
                <img alt="" src="{products.appetizer02.picture}" /> 
                <p class="name">{products.appetizer02.name}</p>
                <p class="price">${(products.appetizer02.price*0.01).toFixed(2)}</p>
            </div>
            <div class="list">
                <img alt="" src="{products.appetizer03.picture}" /> 
                <p class="name">{products.appetizer03.name}</p>
                <p class="price">${(products.appetizer03.price*0.01).toFixed(2)}</p>
            </div>
        </div>
        <div id="b">
            <div class="list">
                <img alt="" src="{products.appetizer04.picture}" /> 
                <p class="name">{products.appetizer04.name}</p>
                <p class="price"p>${(products.appetizer04.price*0.01).toFixed(2)}</p>
            </div>
            <div class="list">
                <img alt="" src="{products.appetizer05.picture}" /> 
                <p class="name">{products.appetizer05.name}</p>
                <p class="price">${(products.appetizer05.price*0.01).toFixed(2)}</p>
            </div>
            <div id="defaultList" class="list">
                <img alt="" src="{defaultPic}" /> 
                <p class="cheese">Cheese Stick</p>
                <p class="name">{products.appetizer06.name}</p>
                <p class="price">${(products.appetizer06.price*0.01).toFixed(2)}</p>
            </div>
        </div>
    </div>
</section>

<style>
    * { margin: 0; padding: 0; box-sizing: border-box; } 
    a { text-decoration: none; color:inherit; }
    img { vertical-align: middle; border: none; }
    h1, h2 { font-weight: normal; }
    
    #nav2{
        display: flex;
        text-align: center;
        align-items: center;
        margin-bottom: 30px;
        margin-left: 30px;
    }
    #nav2 a{
        width: 80px;
        height: 50px;
        font-size: 30px;
        font-weight: bold;
        text-align: center;
        align-items: center;
        border-radius: 5px;
        box-shadow: 2px 2px 2px 2px rgb(228, 226, 226);
    }
    #nav2 .title {
        font-size: 40px;
        font-weight: bold;
        padding: 0 30px;
    }
    #nav2 .dot {
        padding-right: 30px;
        font-weight: 500;
        color: gray;
    }
    #nav2 .subtitle{
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
    #a, #b{
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
    #defaultList{
        position: relative !important;
    }
    .cheese {
        position: absolute;
        top: 0%;
        left: 5%;
        color: white;
        font-weight: bold;
        font-size: 3rem !important;
    }

    @media screen and (max-width:1199px) {
    /* 테블릿 가로 */
        .list {
            margin-bottom: 40px;
        }
        .cheese {
            font-size: 2.5rem !important;
        }
    }

    @media screen and (max-width:899px) {
    /* 모바일 가로, 테블릿 세로 */
        .list img {
            height: 80% !important;
        }
        .cheese {
            font-size: 2rem !important;
        }

        #nav2 {
            margin-left: 0;
        }
        #nav2 .title {
            font-size: 2rem;
            font-weight: bold;
            padding: 0 1rem;
        }
        #nav2 .dot {
            padding-right: 1rem;
            font-weight: 500;
            color: gray;
        }
        #nav2 .subtitle{
            font-weight: 500;
            color: gray;
        }
    }

    @media screen and (max-width:599px) {
    /* 모바일 세로 */
        #a, #b {
            flex-direction: column;
        }
        .list {
            width: 100%;
            height: 400px !important;
            margin-bottom: 80px;
        }
        .cheese {
            font-size: 2.5rem !important;
        }
        #nav2 a {
            width: 70px;
            font-size: 2rem;
        }
        #nav2 .title {
            font-size: 2rem;
            font-weight: bold;
            padding: 0 1.8rem;
        }
        #nav2 .dot {
            font-size: 0;
        }
        #nav2 .subtitle{
            font-size: 0;
        }
        #nav2 .dot {
            font-size: 0;
        }
        #nav2 .subtitle{
            font-size: 0;
        }
        .list .name {
            font-weight: bold;
        }
    }
</style>