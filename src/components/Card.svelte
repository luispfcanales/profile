<script>
  import Button from './Button.svelte'
</script>

<div class="container-card">
  <div class="container-avatar">
    <img src="https://avatars.githubusercontent.com/u/66489348?s=96&v=4" alt="avatar">
  </div>
  <h1>Web Developer</h1>
  <br/>
  <h2>Luis Angel Pfuño Canales</h2>
  <Button/>
</div>

<style>
  .container-card{
    box-sizing:border-box;
    margin:0;
    padding:0;
    width:360px;
    display:flex;
    flex-direction:column;
    justify-content:center;
    align-items:center;
    border-radius:16px;
    box-shadow:0 0 12px rgba(1,1,1,.15);
    transition:.3s;
    backdrop-filter:blur(10px);
  }
  .container-card:hover{
    box-shadow:0 0 12px rgba(1,1,1,.15),
      0 0 15px rgba(1,1,1,.15);
  }
  .container-avatar{
    width:100px;
    height:100px;
    margin-top:1rem;
    background:var(--bg-color-avatar);
    border-radius:21% 79% 82% 18% / 50% 33% 67% 50%;
    overflow:hidden;
    box-shadow:0 0 12px rgba(1,1,1,.3);
  }
  h1{
    margin-top:1rem;
    font-family:'Satisfy',cursive;
    font-size:2.2rem;
    color:var(--text-color);
    text-shadow:0 0 7px var(--text-color);
  }
  br{
    content:" ";
    width: 70%;
    border-bottom:2px solid var(--text-color);
  }
  h2{
    margin-top:.5rem;
    color:#111;
    font-family:'Satisfy';
    font-size:1.4rem;
    text-shadow:0 0 7px rgba(1,1,1,.5);
  }

</style>
