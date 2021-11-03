<script>
    export let text;
    const handleClick = () =>{
        document.getElementById("container").style.display = "none";
};
</script>
<div id="container" class="container">
    <div class="text">
        <p>{text}</p>
    </div>
    <div>
        <button on:click={handleClick}>Hide text</button>
    </div>
</div>

<style>
    button{
        background-color: grey;
        padding: 10px;
        border-radius: 5%;
        border: none;
        color: white;
    }
</style>