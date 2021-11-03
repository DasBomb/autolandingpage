<script>
    export let btn1 = 'btn1',
    btn2 = 'btn2',
    btn3 = 'btn3',
    href1 = '',
    href2 = '',
    href3='';

</script>


<div class="container">
    <div class="btn">
        <a href="#{btn1}">{btn1}</a>
    </div>
    <div class="btn">
        <a href={href2}>{btn2}</a>
    </div>
    <div class="btn">
        <a href="{href3}">{btn3}</a>
    </div>
</div>

<style>
    .container{
        display: flex;
        flex-direction: row;
        justify-content: flex-end;
        font-family: sans-serif;
    }

    .btn{
        margin-left: 1em;
        background-color: grey;
        padding: 10px;
        border-radius: 5%;
    }

    a{
        text-decoration: none;
        text-transform: uppercase;
        font-weight: 700;
        letter-spacing: 1px;
        font-size: 13px;
        color: white;
    }
</style>