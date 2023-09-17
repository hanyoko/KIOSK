<script>
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
                
        default: {
            picture: 'https://windowsforum.kr/files/attach/images/2966154/176/607/019/87649558142f291ae09689066ee8f2fc.jpg',
        }
    }
</script>

    <div id="main">
        <div id="nav2">
            <a id="back" href="/"><p>←</p></a>
            <h1 style="padding: 0 30px;">Appetizer</h1>
            <h2 style="padding-right: 30px; font-weight: 500; color: gray;">·</h2>
            <h2 style="font-weight: 500; color: gray;">Salad and Fries</h2>
        </div>

        <div id="a">
            <div class="list">
                <img alt="" src="{products.appetizer01.picture}" />
                <p>{products.appetizer01.name}</p>
                <p>${products.appetizer01.price*0.01}</p>
            </div>
            <div class="list">
                <img alt="" src="{products.appetizer02.picture}" /> 
                <p>{products.appetizer02.name}</p>
                <p>${products.appetizer02.price*0.01}</p>
            </div>
            <div class="list">
                <img alt="" src="{products.appetizer03.picture}" /> 
                <p>{products.appetizer03.name}</p>
                <p>${products.appetizer03.price*0.01}</p>
            </div>
        </div>
        <div id="b">
            <div class="list">
                <img alt="" src="{products.appetizer04.picture}" /> 
                <p>{products.appetizer04.name}</p>
                <p>${products.appetizer04.price*0.01}</p>
            </div>
            <div class="list">
                <img alt="" src="{products.appetizer05.picture}" /> 
                <p>{products.appetizer05.name}</p>
                <p>${products.appetizer05.price*0.01}</p>
            </div>
            <div class="list">
                <img id="cheeseImg" alt="Cheese Stick" style="font-size: 30px; color: white; font-style: bold;" src="{products.default.picture}" /> 
                <p class="cheese">Cheese Stick</p>
                <p>{products.appetizer06.name}</p>
                <p>${products.appetizer06.price*0.01}</p>
            </div>
        </div>
    </div>

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
            width: 30%;
            height: 300px;
            margin-bottom: 170px;
         
        }
        .list img {
            width: 100%;
            height: 310px !important;
            border-radius: 10px;
            object-fit: fill;
            
        }
        .list p {
            font-size: 30px;
            padding: 10px 0;
            margin-top: 3px;
        }
        #cheeseImg{
            position: relative !important;
        }
        .cheese {
            position: absolute;
            bottom: 19%;
            right: 16%;
            color: white;
            font-weight: bold;
            font-size: 50px !important;
        }
    </style>