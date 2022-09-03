<script>
  import Card from './components/Card.svelte'
  import Circle from './components/Circle.svelte'

</script>

<main>
  <Circle/>
  <Card/>
</main>

<style>
  :root{
    --bg-color:linear-gradient(45deg,#4C3575,#7858A6,#fb6fe2);

    --bg-color-avatar:linear-gradient(25deg,#4C3575,#712B75,#7A0BC0);
    --bg-color-btn:linear-gradient(45deg,#52057B,#712B75,#F10086);

    --text-color-shadow:#680b9c;
    --text-color-primary:#4c0373;

    --size-height-btn:3rem;
    --bg-color-circle:radial-gradient(#F10086,#f51196);
    --bg-color-circle-shadow:#F10086;
    --bg-color-circle2:#52057B;
    --bg-color-circle2-shadow:#680b9c;
  }
  main{
    position:relative;
    margin:0;
    padding:0;
    width:100vw;
    height:100vh;
    background:var(--bg-color);
    display:flex;
    justify-content:center;
    align-items:center;
    overflow:hidden;
  }
</style>
