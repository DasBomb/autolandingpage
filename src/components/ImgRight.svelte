<script>
	export let imgSrc;

	let imgRightText;
	$: imgRightText;
</script>

<div class="container">
	<img class="imgRight" src={imgSrc} alt="" />
	<input type="text" placeholder="Text for right photo" bind:value={imgRightText} />
	<p class="txtLeft">{imgRightText}</p>
</div>

<style>
	.container {
		display: flex;
        align-items: center;
	}
	.imgRight {
		width: 100%;
		float: right;
        margin-right: 8%;
	}
	.txtRight {
		text-align: right;
        width: 160%;
        margin-left: 8%;
	}
</style>
