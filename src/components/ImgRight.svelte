<script>
	export let textArea;
	export let imgSrc2;
</script>

<div class="container">
	<p class="txtRight">{textArea}</p>
	<img class="imgRight" src={imgSrc2} alt="" />
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
