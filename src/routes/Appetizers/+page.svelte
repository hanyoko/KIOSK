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
  }
}
</script>


<div id="wrap">
    <nav id="nav">
        <li class="li" style="width: 17%">English<img src="./status/img/chevron-down.png" alt=""></li>
        <li class="li" style="width: 24%">Call Waiter</li>
        <li class="li" style="width: 24%">View Bill</li>
        <li class="li" style="width: 24%">My Cart</li>
        <li style="width: 11%">0</li>
    </nav>

    <div id="main">
        <div id="nav2">
            <a href="/"><p>←</p></a>
            <h1>Appetizer</h1>
            <h2> · Salad and Fries</h2>
        </div>
        <div id="a">
            <div class="list">
                <img alt="" src="{products.appetizer01.picture}" />
                <p>{products.appetizer01.name}</p>
                <p>{products.appetizer01.price}</p>
            </div>
            <div class="list">
                <img alt="" src="{products.appetizer02.picture}" /> 
                <p>{products.appetizer02.name}</p>
                <p>{products.appetizer01.price}</p>
            </div>
            <div class="list">
                <img alt="" src="{products.appetizer03.picture}" /> 
                <p>{products.appetizer03.name}</p>
                <p>{products.appetizer01.price}</p>
            </div>
        </div>
        <div id="b">
            <div class="list">
                <img alt="" src="{products.appetizer04.picture}" /> 
                <p>{products.appetizer04.name}</p>
                <p>{products.appetizer01.price}</p>
            </div>
            <div class="list">
                <img alt="" src="{products.appetizer05.picture}" /> 
                <p>{products.appetizer05.name}</p>
                <p>{products.appetizer01.price}</p>
            </div>
            <div class="list">
                <!-- <img alt="" src="{products.appetizer06.picture}" />  -->
                <p>{products.appetizer06.name}</p>
                <p>{products.appetizer01.price}</p>
            </div>
        </div>
    </div>
</div>

<style>
    * { margin: 0; padding: 0; box-sizing: border-box; }
    a { text-decoration: none; color:inherit; }
    li { list-style: none; }
    img { vertical-align: top; border: none; }
    h1, h2 { font-weight: normal; }
    
        #wrap{
            width: 100%;
        }
        #nav{
            line-height: 80px;
            font-size: 35px;
            display: flex;
            justify-content: space-around;
            text-align: center;
            align-items: center;
            background: black;
            color: white;
            width: 100%;
        }
        .li {
            border-right: 1px dotted gray;
        }
        #nav2{
            display: flex;
            text-align: center;
            align-items: center;
        }
        #nav2 h1{
            padding: 0 20px;
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
        }
        .list {
            /* margin: 25px 0; */
            display: flex;
            flex-direction: column;
            text-align: center;
            align-items: center;
            border-radius: 10%;
            width: 100%;
        }
        .list p {
            margin: 30px 0;
            padding-top: 180px;
            font-size: 30px;
        }
    </style>