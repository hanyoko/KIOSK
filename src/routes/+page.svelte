<script>
    const categories = {
        mockCategory01: {
            description: 'Salad and fries',
            id: 'mockCategory01',
            name: 'Appetizers',
            picture: 'https://picsum.photos/300/200.webp',
            productOrder: [
            'appetizer01',
            'appetizer02',
            'appetizer03',
            'appetizer04',
            'appetizer05',
            'appetizer06',
            ],
        },
        mockCategory02: {
            id: 'mockCategory02',
            name: 'Meat Pasta',
            picture: 'https://picsum.photos/300/200.webp',
            productOrder: [
            'meatPasta01',
            'meatPasta02',
            'meatPasta03',
            'meatPasta04',
            'meatPasta05',
            'meatPasta06',
            'meatPasta07',
            'meatPasta08',
            ],
        },
        mockCategory03: {
            id: 'mockCategory03',
            name: 'Wine',
            picture: 'https://picsum.photos/300/200.webp',
            productOrder: ['wine01', 'wine02', 'wine03', 'wine04'],
        },
        mockCategory04: {
            id: 'mockCategory04',
            name: 'Lunch Menu',
            picture: 'https://picsum.photos/300/200.webp',
            productOrder: ['appetizer01', 'meatPasta01', 'meatPasta06', 'wine01'],
        },
        mockCategory05: {
            id: 'mockCategory05',
            name: 'Vegetarian Pasta',
            picture: 'https://picsum.photos/300/200.webp',
            productOrder: ['appetizer04', 'appetizer05'],
        },
        mockCategory06: {
            id: 'mockCategory06',
            name: 'Special Menu',
            picture: 'https://picsum.photos/300/200.webp',
            productOrder: ['wine02', 'wine03'],
        },
        mockCategory07: {
            id: 'mockCategory07',
            name: `Kid's Menu`,
            picture: 'https://picsum.photos/300/200.webp',
            productOrder: ['appetizer01', 'meatPasta05', 'meatPasta06', 'meatPasta07', 'meatPasta08'],
        },
        mockCategory08: {
            id: 'mockCategory08',
            name: 'Beverages',
            picture: 'https://picsum.photos/300/200.webp',
            productOrder: [],
        },
        mockCategory09: {
            id: 'mockCategory09',
            name: 'Pizza',
            picture: 'https://picsum.photos/300/200.webp',
            productOrder: [],
        },
        mockCategory10: {
            id: 'mockCategory10',
            name: 'Steak',
            picture: 'https://picsum.photos/300/200.webp',
            productOrder: [],
        },
        mockCategory11: {
            id: 'mockCategory11',
            name: 'Chicken Pasta',
            picture: 'https://picsum.photos/300/200.webp',
            productOrder: [],
        },
        mockCategory12: {
            id: 'mockCategory12',
            name: 'Seafood Pasta',
            picture: 'https://picsum.photos/300/200.webp',
            productOrder: [],
        },
        mockCategory13: {
            id: 'mockCategory13',
            name: 'Take Out Only',
            picture: 'https://picsum.photos/300/200.webp',
            productOrder: [],
        },
        mockCategory14: {
            id: 'mockCategory14',
            name: 'Spicy',
            picture: 'https://picsum.photos/300/200.webp',
            productOrder: [],
        },
        mockCategory15: {
            id: 'mockCategory15',
            name: 'Beer',
            picture: 'https://picsum.photos/300/200.webp',
            productOrder: [],
        },
        mockCategory16: {
            id: 'mockCategory16',
            name: 'Dessert',
            picture: 'https://picsum.photos/300/200.webp',
            productOrder: [],
        },
    }
</script>

<section id="wrap">
    <div id="main">
        <div id="a">
            <a href="/Appetizers" class="list">
                <div>
                    <img alt="" src="{categories.mockCategory01.picture}" />
                    <p>{categories.mockCategory01.name}</p>
                </div>
            </a>
            <a href="/Meat_Pasta" class="list">
                <div>
                    <img alt="" src="{categories.mockCategory02.picture}" /> 
                    <p>{categories.mockCategory02.name}</p>
                </div>
            </a>
            <a href="/Wine" class="list">
                <div>
                    <img alt="" src="{categories.mockCategory03.picture}" /> 
                    <p>{categories.mockCategory03.name}</p>
                </div>
            </a>
            <div class="list">
                <img alt="" src="{categories.mockCategory04.picture}" /> 
                <p>{categories.mockCategory04.name}</p>
            </div>
        </div>
        <div id="b">
            <div class="list">
                <img alt="" src="{categories.mockCategory05.picture}" /> 
                <p>{categories.mockCategory05.name}</p>
            </div>
            <div class="list">
                <img alt="" src="{categories.mockCategory06.picture}" /> 
                <p>{categories.mockCategory06.name}</p>
            </div>
            <div class="list">
                <img alt="" src="{categories.mockCategory07.picture}" /> 
                <p>{categories.mockCategory07.name}</p>
            </div>
            <div class="list">
                <img alt="" src="{categories.mockCategory08.picture}" /> 
                <p>{categories.mockCategory08.name}</p>
            </div>
        </div>
        <div id="c">
            <div class="list">
                <img alt="" src="{categories.mockCategory09.picture}" /> 
                <p>{categories.mockCategory09.name}</p>
            </div>
            <div class="list">
                <img alt="" src="{categories.mockCategory10.picture}" /> 
                <p>{categories.mockCategory10.name}</p>
            </div>
            <div class="list">
                <img alt="" src="{categories.mockCategory11.picture}" /> 
                <p>{categories.mockCategory11.name}</p>
            </div>
            <div class="list">
                <img alt="" src="{categories.mockCategory12.picture}" /> 
                <p>{categories.mockCategory12.name}</p>
            </div>
        </div>
        <div id="d">
            <div class="list">
                <img alt="" src="{categories.mockCategory13.picture}" /> 
                <p>{categories.mockCategory13.name}</p>
            </div>
            <div class="list">
                <img alt="" src="{categories.mockCategory14.picture}" /> 
                <p>{categories.mockCategory14.name}</p>
            </div>
            <div class="list">
                <img alt="" src="{categories.mockCategory15.picture}" /> 
                <p>{categories.mockCategory15.name}</p>
            </div>
            <div class="list">
                <img alt="" src="{categories.mockCategory16.picture}" /> 
                <p>{categories.mockCategory16.name}</p>
            </div>
        </div>
    </div>
</section>



<style>
    * { margin: 0; padding: 0; box-sizing: border-box; font-family: sans-serif, "맑은고딕"; }
    a { text-decoration: none; color:inherit; }
    img { vertical-align: middle; border: none; }

    #wrap{
        width: 100%;
    }
    #main {
        width: 100%;
        height: 100vh;
        padding: 30px;
        display: flex;
        flex-direction: column;
    }
    #a, #b, #c, #d{
        width: 100%;
        display: flex;
        justify-content: space-around;
        margin-bottom: 3rem;
    }
    #a {
        margin-top: 20px;
    }

    .list {
        margin: 25px 0;
        background: rgb(247, 240, 240);
        display: flex;
        flex-direction: column;
        text-align: center;
        align-items: center;
        border-radius: 10%;
        width: 20%;
        height: 90%;
        position: relative;
    }
    .list img {
        border: 1;
        border-radius: 100%;
        width: 70%;
        height: 70%;
        object-fit: cover;
        position: absolute;
        top: -8%;
        left: 15%;
    }
    .list p {
        margin: 30px 0;
        padding-top: 200px;
        font-size: 30px;
        font-weight: bold;
    }

    @media screen and (max-width:1199px) {
    /* 테블릿 가로 */
        #a, #b, #c, #d {
            width: 100%;
            display: flex;
            justify-content: space-around;
            margin-bottom: 0;
        }
        .list {
            width: 21%;
            height: 83%;
            margin: 0;
        }
        .list img {
            width: 70%;
            height: 70%;
            top: -8%;
            left: 15%;
        }
        .list p {
            padding-top: 100px;
            padding-bottom: 40px;
            font-size: 25px;
            font-weight: bold;
        }
    }

    @media screen and (max-width:899px) {
    /* 모바일 가로, 테블릿 세로 */
        .list {
            width: 21%;
            height: 88%;
        }
        .list img {
            width: 70%;
            height: 70%;
            top: -8%;
            left: 15%;
        }
        .list p {
            padding-top: 90px;
            padding-bottom: 10px;
            font-size: 19px;
            font-weight: bold;
        }
    }

    @media screen and (max-width:599px) {
    /* 모바일 세로 */
        #a, #b, #c, #d {
            flex-direction: column;
        }
        #a {
            margin-top: 0;
        }
        .list {
            text-align: center;
            width: 100%;
            height: 50%;
            margin: 40px 0;
        }
        .list img {
            border-radius: 8%;
            width: 70%;
            height: 70%;
            top: -3%;
            left: 15%;
        }
        .list p {
            margin: 30px 0;
            padding-top: 210px;
            font-size: 30px;
            font-weight: bold;
        }
    }
</style>