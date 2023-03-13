<script>
  import Avatar from "../components/Avatar.svelte";
  import Button from "../components/Button.svelte";
  import Line from "../components/Line.svelte";
  import Modal from "../components/Modal.svelte";
  import Navbar from "../components/Navbar.svelte";
  import TypeWritter from "../components/TypeWritter.svelte";
  import Typing from "../wrapper/Typing.svelte";

  let modalActive = false;
  const modalHandler =()=>{modalActive = !modalActive} 
</script>

<svelte:head>
  <title>Profile</title>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Noto+Serif+Lao:wght@300&display=swap" rel="stylesheet">
</svelte:head>

<container>
  <Navbar/>
  <Line/>

  <div>
    <Typing>
      <TypeWritter/>
      <Button text={"Suscribete"} {modalHandler}/>
    </Typing>
    <Avatar/>
  </div>
</container>
<Modal 
  {modalActive} 
  {modalHandler}
  blureffect={true}
/>

<style>
  container{
    width:100vw;
    box-sizing:border-box;
    display:flex;
    flex-direction:column;
    width:1024px;
  }
  div{
    margin-top:3rem;
    display:flex;
    gap:2rem;
    align-items:center;
  }
@media (max-width:1024px){
  div{
    flex-direction:column-reverse;
    justify-content:center;
  }
  container{
    margin:0 2rem;
    align-items:center;
  }
}
</style>
