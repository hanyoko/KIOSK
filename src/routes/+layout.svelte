<script>
    const languages = [{name: 'English'}, {name: '한국어'}]
    const tableNumber = '12'

    import lan from '$lib/img/chevron-down.png';
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
    <!-- <select id="languageSelector" class="li" style="width: 17%">
        <option value="en">English</option>
        <option value="ko" selected>한국어</option>
    </select>-->
    English<img alt="" src={lan} />
    </li> 
    <li class="li call">
        <button style="cursor: pointer;" on:click={handleAlert}>
            <img alt="" src={call} />Call Waiter
        </button>
    </li>
    <li class="li bill"><img alt="" src={bill} />View Bill</li>
    <li class="li cart"><img alt="" src={cart} />My Cart<p style="color: white;">0</p></li>
    <li class="table"><img alt="" src={table} />{tableNumber}</li>
</nav>

<slot></slot>

<style>
    * { margin: 0; padding: 0; box-sizing: border-box; }
    li { list-style: none; }
    img { vertical-align: middle; border: none; }
    
    #nav{
        height: 80px;
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
    }
    #nav img {
        width: 30px;
        height: 30px;
        margin: 0 15px;
    }
    #nav button {
        font-size: 27px;
        background: black;
        color: white;
        border: none;
    }
    #nav .lan {
        width: 17%;
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
    #nav .cart p{
        width: 40px;
        margin: 0 15px;
        border-radius: 100%;
        background-color: gray;
    }
    #nav .table {
        width: 11%;
        font-size: 40px; 
        font-weight: bold;
    }
    .li {
        border-right: 1px solid gray;
    }
</style>