<script>
	export let textArea;
	export let imgSrc;
</script>

<div class="container">
	<img class="imgLeft" src={imgSrc} alt="" />
	<p class="txtLeft">{textArea}</p>
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