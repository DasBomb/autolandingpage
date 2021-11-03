<script>
	export let textArea;
	export let imgSrc;

	let imgLeftText;
	$: imgLeftText;
</script>

<div class="container">
	<img class="imgLeft" src={imgSrc} alt="" />
	<input type="text" placeholder="leftImgText" bind:value={imgLeftText} />
	<p class="txtLeft">{imgLeftText}</p>
	
</div>

<style>
	.container {
		display: flex;
        align-items: center;
	}
	.imgLeft {
		width: 100%;
		float: left;
        margin-left: 8%;
	}
	.txtLeft {
		text-align: left;
        width: 160%;
        margin-right: 8%;
	}
</style>