<script>
    const tableNumber = '12'

    import call from '$lib/img/notifications_active.png';
    import bill from '$lib/img/receipt.png';
    import cart from '$lib/img/shopping_cart.png';
    import table from '$lib/img/table.png';

    function handleAlert() {
        alert("Waiter Called");
    }

</script>

<nav id="nav">
    <li class="li lan">
        <select id="languageSelector">
            <option value="en" selected>English</option>
            <option value="ko" >한국어</option>
            <option value="ja" >にほんご</option>
            <option value="ch" >中國語</option>
        </select>
    </li> 
    <li class="li call">
        <button style="cursor: pointer;" on:click={handleAlert}>
            <img alt="" src={call} />Call Waiter
        </button>
    </li>
    <li class="li bill"><img alt="" src={bill} />View Bill</li>
    <li class="li cart"><img alt="" src={cart} />My Cart<span class="circle">0</span></li>
    <li class="table"><img alt="" src={table} />{tableNumber}</li>
</nav>

<slot />

<style>
    * { margin: 0; padding: 0; box-sizing: border-box; font-family: sans-serif, "맑은고딕"; }
    li { list-style: none; }
    img { vertical-align: middle; border: none; }
    
    #nav {
        height: 70px;
        font-size: 0;
        display: flex;
        justify-content: space-around;
        text-align: center;
        align-items: center;
        background: black;
        color: white;
        width: 100%;
    }
    #nav li {
        align-items: center;
        height: 40px;
        font-size: 27px;
    }
    #nav img {
        width: 35px;
        height: 35px;
        margin: 0 15px;
    }
    #nav button {
        width: 80%;
        height: 40px;
        font-size: 27px;
        background: black;
        color: white;
        border: none;
    }
    #nav .lan {
        width: 16%;
    }
    #languageSelector {
        font-size: 27px;
        border: 0;
        background-color: black;
        color: white;
        width: 70%;
        height: 40px;
        text-align: center;
        cursor: pointer;
    }

    #nav .call {
        width: 24%;
    }
    #nav .bill {
        width: 24%;
        color: gray;
    }
    #nav .cart {
        width: 24%;
        color: gray;
    }
    #nav .cart .circle {
        display: inline-block;
        width: 40px;
        height: 40px;
        margin-left: 10px; 
        border-radius: 50%;
        background-color: gray;
        color: white;
    }
    #nav .table {
        width: 12%;
        font-weight: bold;
    }
    .li {
        border-right: 1px solid gray;
    }

    @media screen and (max-width:1199px) {
    /* 테블릿 가로 */
        #nav {
            height: 70px;
        }
        #nav button {
            height: 40px;
            font-size: 23px;
        }
    }

    @media screen and (max-width:899px) {
    /* 모바일 가로, 테블릿 세로 */
        #nav {
            line-height: 40px;
        }
        #nav li, #languageSelector {
            font-size: 18px;
        }
        #nav .lan {
            width: 16%;
        }
        #nav .call {
            width: 25%;
        }
        #nav .bill {
            width: 22%;
        }
        #nav .cart {
            width: 24%;
        }
        #nav .table {
            width: 13%;
        }
        #nav img {
            width: 30px;
            height: 30px;
            margin: 0 10px;
        }
        #nav button {
            font-size: 18px;
        }
    }

    @media screen and (max-width:599px) {
    /* 모바일 세로 */
        #nav img {
            width: 35px;
            height: 35px;
        }
        #nav .lan {
            width: 26%;
        }
        #nav .call {
            width: 18%;
            text-align: center;
            position: relative;
        }
        #nav .call button {
            position: absolute;
            top: 0;
            left: 0;
            font-size: 0;
            width: 100%;
        }
        #nav .bill {
            width: 18%;
            font-size: 0;
        }
        #nav .cart {
            width: 18%;
            font-size: 0;
        }
        #nav .cart .circle {
            display: none;
        }
        #nav .table {
            width: 18%;
            font-size: 0;
        }
        #nav .table img {
            width: 40%;
            height: 70%;
        }
    }
</style>