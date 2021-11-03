<script>
	export let textArea = "asdakjdhasdk hahdka hdakjsdh akdha skjdad";
	export let imgSrc = watermelon;
	import watermelon from '../assets/watermelon.jpg';
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