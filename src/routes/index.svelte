<script>
    import Nav from '../components/Nav.svelte'
    import Text from '../components/Text.svelte'
    import TextWithBtn from '../components/TextWithBtn.svelte'
    import Carousel from '../components/Carousel.svelte'
    import ContactForm from '../components/ContactForm.svelte'
    import ImgLeft from '../components/ImgLeft.svelte'
    import ImgRight from '../components/ImgRight.svelte'

let btn1, title;
$: btn1, title;

</script>


<input type="text" placeholder="btn1 text" bind:value={btn1}>

<input type="text" placeholder="title text" bind:value={title}>

<Nav {btn1}></Nav>
<img src="" alt=""> /* Här ska avataren vara */
<h1>{title}</h1>
<Text></Text>
<ImgRight></ImgRight>
<ImgLeft></ImgLeft>
<Carousel></Carousel>
<TextWithBtn></TextWithBtn>
<ContactForm></ContactForm>
