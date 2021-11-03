<script>
    import Nav from '../components/Nav.svelte'
    import Text from '../components/Text.svelte'
    import TextWithBtn from '../components/TextWithBtn.svelte'
    import Carousel from '../components/Carousel.svelte'
    import ContactForm from '../components/ContactForm.svelte'
    import ImgLeft from '../components/ImgLeft.svelte'
    import ImgRight from '../components/ImgRight.svelte'

let btn1, color1, color2;
$: btn1, color1, color2;
</script>


<input type="text" placeholder="btn1 text" bind:value={btn1}><br>


<label>Choose a background color for the first section: 
    <input type="color" placeholder="color1" bind:value={color1}></label>
<label>Choose a background color for the second section:
    <input type="color" placeholder="color1" bind:value={color2}> </label>

<Nav {btn1}></Nav>
<img src="" alt=""> /* Här ska avataren vara */
<h1>Title</h1>
<Text></Text>
<div style="background-color: {color1};">
<ImgRight></ImgRight>
</div>
<div style="background-color: {color2};">
<ImgLeft></ImgLeft>
</div>
<Carousel></Carousel>
<TextWithBtn></TextWithBtn>
<ContactForm></ContactForm>

