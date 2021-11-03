<script>
    import Nav from '../components/Nav.svelte'
    import Text from '../components/Text.svelte'
    import TextWithBtn from '../components/TextWithBtn.svelte'
    import Carousel from '../components/Carousel.svelte'
    import ContactForm from '../components/ContactForm.svelte'
    import ImgLeft from '../components/ImgLeft.svelte'
    import ImgRight from '../components/ImgRight.svelte'

    import Option1 from '../components/pics/Option1.jpg'
    import Option2 from '../components/pics/Option2.jpg'
    import Option3 from '../components/pics/Option3.jpg'
    

let btn1, btn2, btn3, textArea, title, color1, color2, imgSrc, imgSrc2;
$: btn1, btn2, btn3, textArea, title, color1, color2, imgSrc, imgSrc2;


</script>

<label for="leftPic">Choose your left picture:</label>
<select name="leftPic" bind:value={imgSrc}>
    <option value={Option1}>Bild 1</option>
    <option value={Option2}>Bild 2</option>
    <option value={Option3}>Bild 3</option>
</select>

<label for="rightPic">Choose your right picture:</label>
<select name="rightPic" bind:value={imgSrc2}>
    <option value={Option1}>Bild 1</option>
    <option value={Option2}>Bild 2</option>
    <option value={Option3}>Bild 3</option>
</select>



<input type="text" placeholder="Name the first section" bind:value={btn1}>
<input type="text" placeholder="Name the second section" bind:value={btn2}>
<input type="text" placeholder="Namethe third section" bind:value={btn3}>

<label>Choose a background color for the first section: 
    <input type="color" placeholder="color1" bind:value={color1}></label>
<label>Choose a background color for the second section:
    <input type="color" placeholder="color1" bind:value={color2}> </label>


<textarea name="" id="" cols="30" rows="10" bind:value={textArea}></textarea>
<input type="text" placeholder="title text" bind:value={title}>

<Nav {btn1} {btn2} {btn3} ></Nav>
<img src="" alt=""> /* Här ska avataren vara */
<h1>{title}</h1>
<Text {textArea}></Text>
<ImgRight {imgSrc2}></ImgRight>
<ImgLeft {imgSrc}></ImgLeft>

<div style="background-color: {color1};">

</div>
<div style="background-color: {color2};">

</div>
<Carousel></Carousel>
<TextWithBtn></TextWithBtn>
<ContactForm></ContactForm>
