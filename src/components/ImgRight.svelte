<script>
	export let textArea2;
	export let imgSrc;
</script>

<div class="container">
	<p class="txtRight">{textArea2}</p>
	<img class="imgRight" src={imgSrc} alt="" />
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
