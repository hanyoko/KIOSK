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
                
        // default: {
        //     picture: '',
        // }
    }

</script>

<section>
    <div id="main">
        <div id="nav2">
            <a id="back" href="/"><p>←</p></a>
            <h1 style="font-size: 40px; font-weight: bold; padding: 0 30px;">Appetizer</h1>
            <h2 style="padding-right: 30px; font-weight: 500; color: gray;">·</h2>
            <h2 style="font-weight: 500; color: gray;">Salad and Fries</h2>
        </div>

        <div id="a">
            <div class="list">
                <img alt="" src="{products.appetizer01.picture}" />
                <p>{products.appetizer01.name}</p>
                <p class="price">${(products.appetizer01.price*0.01).toFixed(2)}</p>
            </div>
            <div class="list">
                <img alt="" src="{products.appetizer02.picture}" /> 
                <p>{products.appetizer02.name}</p>
                <p class="price">${(products.appetizer02.price*0.01).toFixed(2)}</p>
            </div>
            <div class="list">
                <img alt="" src="{products.appetizer03.picture}" /> 
                <p>{products.appetizer03.name}</p>
                <p class="price">${(products.appetizer03.price*0.01).toFixed(2)}</p>
            </div>
        </div>
        <div id="b">
            <div class="list">
                <img alt="" src="{products.appetizer04.picture}" /> 
                <p>{products.appetizer04.name}</p>
                <p class="price"p>${(products.appetizer04.price*0.01).toFixed(2)}</p>
            </div>
            <div class="list">
                <img alt="" src="{products.appetizer05.picture}" /> 
                <p>{products.appetizer05.name}</p>
                <p class="price">${(products.appetizer05.price*0.01).toFixed(2)}</p>
            </div>
            <div id="cheeseImg" class="list">
                <img alt="" src="{defaultPic}" /> 
                <p class="cheese">Cheese Stick</p>
                <p>{products.appetizer06.name}</p>
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
        #cheeseImg{
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
    </style>