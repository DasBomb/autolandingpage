<script>
    import Nav from '../components/Nav.svelte'
    import Text from '../components/Text.svelte'
    import TextWithBtn from '../components/TextWithBtn.svelte'
    import Carousel from '../components/Carousel.svelte'
    import ContactForm from '../components/ContactForm.svelte'
    import ImgLeft from '../components/ImgLeft.svelte'
    import ImgRight from '../components/ImgRight.svelte'


let btn1, btn2, btn3, textArea, title;
$: btn1, btn2, btn3, textArea, title;


</script>


<input type="text" placeholder="Name the first section" bind:value={btn1}>
<input type="text" placeholder="Name the second section" bind:value={btn2}>
<input type="text" placeholder="Namethe third section" bind:value={btn3}>


<textarea name="" id="" cols="30" rows="10" bind:value={textArea}></textarea>
<input type="text" placeholder="title text" bind:value={title}>

<Nav {btn1} {btn2} {btn3} ></Nav>
<img src="" alt=""> /* Här ska avataren vara */
<h1>{title}</h1>
<Text {textArea}></Text>

<ImgRight></ImgRight>
<ImgLeft></ImgLeft>
<Carousel></Carousel>
<TextWithBtn></TextWithBtn>
<ContactForm></ContactForm>
