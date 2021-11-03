<script>
	import Nav from '../components/Nav.svelte';
	import Text from '../components/Text.svelte';
	import TextWithBtn from '../components/TextWithBtn.svelte';
	import Carousel from '../components/Carousel.svelte';
	import ContactForm from '../components/ContactForm.svelte';
	import ImgLeft from '../components/ImgLeft.svelte';
	import ImgRight from '../components/ImgRight.svelte';

	import Option1 from '../components/pics/Option1.jpg';
	import Option2 from '../components/pics/Option2.jpg';
	import Option3 from '../components/pics/Option3.jpg';

	let btn1, btn2, btn3, textArea, title, color1, color2, imgSrc, imgSrc2, textArea2, textArea3;
	$: btn1, btn2, btn3, textArea, title, color1, color2, imgSrc, imgSrc2, textArea2, textArea3;
</script>

<div class="form">
	<input type="text" placeholder="title text" bind:value={title} />

	<textarea
		name=""
		id=""
		cols="30"
		rows="10"
		bind:value={textArea}
		placeholder="write some text plz"
	/>
	<div class="chooseImg">
		<label for="leftPic">Choose your left picture:</label>
		<select name="leftPic" bind:value={imgSrc}>
			<option value={Option1}>Bild 1</option>
			<option value={Option2}>Bild 2</option>
			<option value={Option3}>Bild 3</option>
		</select>

		<input type="text" placeholder="left" bind:value={textArea3} style="margin-bottom: 1em;" />

		<label for="rightPic">Choose your right picture:</label>
		<select name="rightPic" bind:value={imgSrc2}>
			<option value={Option1}>Bild 1</option>
			<option value={Option2}>Bild 2</option>
			<option value={Option3}>Bild 3</option>
		</select>
		<input type="text" placeholder="right" bind:value={textArea2} style="margin-bottom: 1em;"/>
	</div>
	<input type="text" placeholder="Name the first section" bind:value={btn1} />
	<input type="text" placeholder="Name the second section" bind:value={btn2} />
	<input type="text" placeholder="Name the third section" bind:value={btn3} />

	<label
		>Choose a background color for the first section:
		<input type="color" placeholder="color1" bind:value={color1} /></label
	>
	<label
		>Choose a background color for the second section:
		<input type="color" placeholder="color1" bind:value={color2} />
	</label>
</div>

<div class="outputContainer">
	<Nav {btn1} {btn2} {btn3} />
    <div id="{btn1}" class="sectionOne">
	<h1>{title}</h1>
	<Text {textArea} />
</div>
	<ImgRight {textArea2} {imgSrc2} />
	<ImgLeft {textArea3} {imgSrc} />

	<div style="background-color: {color1};" />
	<div style="background-color: {color2};" />

	<Carousel />
	<TextWithBtn />
	<ContactForm />
</div>

<style>
	.form {
		display: flex;
		flex-direction: column;
		margin: 1em;
	}
	.chooseImg {
		display: flex;
		flex-direction: column;
		justify-content: space-between;
		margin: 1em auto;
		padding: 1em;
	}
	.outputContainer {
		
	}
	label {
		margin-bottom: 1px;
	}
</style>
