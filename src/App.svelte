<script>
  import Profile from "./containers/Profile.svelte";

</script>

<main>
  <Profile></Profile>
</main>

<style>
  :root{
    --size-mobile:1024px;
    --bg-body-color:#16212c;
    --bg-body-color2:#3f4d5a;
    --line-color:#4e657e;
  }
  *{
    margin:0;
    padding:0;
  }
  main{
    position:relative;
    margin:0;
    padding:0;
    box-sizing:border-box;
    width:100vw;
    height:100vh;
    background:var(--bg-body-color);
    display:flex;
    justify-content:center;
  }
</style>
