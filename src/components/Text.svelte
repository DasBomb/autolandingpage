<script>
    export let textArea = 'This is an input text'
</script>

<div class="container">
    <div style="width:80% word-wrap: break-word">
        <p>{textArea}</p>
    </div>
</div>

<style>
    .container{
        display: flex;
        justify-content: center;
        margin: 1em auto;
        font-family: sans-serif;
       
    }
</style>