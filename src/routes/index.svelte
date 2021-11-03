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
    

let btn1, imgSrc, imgSrc2;
$: btn1, imgSrc, imgSrc2;

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

<input type="text" placeholder="btn1 text" bind:value={btn1}>

<Nav {btn1}></Nav>
<img src="" alt=""> /* Här ska avataren vara */
<h1>Title</h1>
<Text></Text>
<ImgRight {imgSrc2}></ImgRight>
<ImgLeft {imgSrc}></ImgLeft>
<Carousel></Carousel>
<TextWithBtn></TextWithBtn>
<ContactForm></ContactForm>