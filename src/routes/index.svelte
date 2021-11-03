<script>
    import Nav from '../components/Nav.svelte'
    import Text from '../components/Text.svelte'
    import TextWithBtn from '../components/TextWithBtn.svelte'
    import Carousel from '../components/Carousel.svelte'
    import ContactForm from '../components/ContactForm.svelte'
    import ImgLeft from '../components/ImgLeft.svelte'
    import ImgRight from '../components/ImgRight.svelte'


let btn1, btn2, btn3, textArea, title, color1, color2;
$: btn1, btn2, btn3, textArea, title, color1, color2;


</script>




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
<div style="background-color: {color1};">
<ImgRight></ImgRight>
</div>
<div style="background-color: {color2};">
<ImgLeft></ImgLeft>
</div>
<Carousel></Carousel>
<TextWithBtn></TextWithBtn>
<ContactForm></ContactForm>
