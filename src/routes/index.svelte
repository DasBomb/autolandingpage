<script>
    import Nav from '../components/Nav.svelte'
    import Text from '../components/Text.svelte'
    import TextWithBtn from '../components/TextWithBtn.svelte'
    import Carousel from '../components/Carousel.svelte'
    import ContactForm from '../components/ContactForm.svelte'
    import ImgLeft from '../components/ImgLeft.svelte'
    import ImgRight from '../components/ImgRight.svelte'

let btn1;
$: btn1;

</script>


<input type="text" placeholder="btn1 text" bind:value={btn1}>

<Nav {btn1}></Nav>
<img src="" alt=""> /* Här ska avataren vara */
<h1>Title</h1>
<Text></Text>
<ImgRight></ImgRight>
<ImgLeft></ImgLeft>
<Carousel></Carousel>
<TextWithBtn></TextWithBtn>
<ContactForm></ContactForm>
