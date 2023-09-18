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

<slot></slot>

<style>
    * { margin: 0; padding: 0; box-sizing: border-box; }
    li { list-style: none; }
    img { vertical-align: middle; border: none; }
    
    #nav{
        height: 8vh;
        font-size: 27px;
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
    }
    #nav img {
        width: 35px;
        height: 35px;
        margin: 0 15px;
    }
    #nav button {
        width: 80%;
        height: 5vh;
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
    }

    #nav .call {
        width: 24%;
    }
    #nav .bill {
        width: 24%;
        color: gray;
    }
    #nav .cart {
        display: flex;
        justify-content: center;
        width: 24%;
        color: gray;
    }
    #nav .cart .circle{
        width: 40px;
        height: 40px;
        margin-left: 10px; 
        border-radius: 50%;
        background-color: gray;
        color: white;
    }
    #nav .table {
        width: 12%;
        font-size: 30px; 
        font-weight: bold;
    }
    .li {
        border-right: 1px solid gray;
    }
</style>