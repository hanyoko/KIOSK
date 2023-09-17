<script>
    const products = {
        wine01: {
            description: '',
            id: 'wine01',
            name: 'House Wine (Red)',
            picture: 'https://picsum.photos/300/200.webp',
            price: 800,
        },
        wine02: {
            description: '',
            id: 'wine02',
            name: 'House Wine (White)',
            picture: 'https://picsum.photos/300/200.webp',
            price: 800,
        },
        wine03: {
            description: '',
            id: 'wine03',
            name: 'Bottle Wine (Red)',
            picture: 'https://picsum.photos/300/200.webp',
            price: 6200,
        },
        wine04: {
            description: '',
            id: 'wine04',
            name: 'Bottle Wine (Red)',
            picture: 'https://picsum.photos/300/200.webp',
            price: 6200,
        },
                
        default: {
            picture: 'https://windowsforum.kr/files/attach/images/2966154/176/607/019/87649558142f291ae09689066ee8f2fc.jpg',
        }
    }
</script>

    <div id="main">
        <div id="nav2">
            <a id="back" href="/"><p>←</p></a>
            <h1 style="padding: 0 30px;">Wine</h1>
            <h2 style="padding-right: 30px; font-weight: 500; color: gray;">·</h2>
            <h2 style="font-weight: 500; color: gray;">Wine</h2>
        </div>

        <div id="a">
            <div class="list">
                <img alt="" src="{products.wine01.picture}" />
                <p>{products.wine01.name}</p>
                <p>${products.wine01.price*0.01}</p>
            </div>
            <div class="list">
                <img alt="" src="{products.wine02.picture}" /> 
                <p>{products.wine02.name}</p>
                <p>${products.wine02.price*0.01}</p>
            </div>
            <div class="list">
                <img alt="" src="{products.wine03.picture}" /> 
                <p>{products.wine03.name}</p>
                <p>${products.wine03.price*0.01}</p>
            </div>
        </div>
        <div id="b">
            <div class="list">
                <img alt="" src="{products.wine04.picture}" /> 
                <p>{products.wine04.name}</p>
                <p>${products.wine04.price*0.01}</p>
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
    </style>