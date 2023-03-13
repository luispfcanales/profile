<script>
  export let modalActive = false;//is visible modal
  export let blureffect = false;//bluer effect in modal
  export let modalHandler; //handler of open and close modal

  import GoX from 'svelte-icons/go/GoX.svelte'

</script>


<style>
  container{
    display:none;
    position:absolute;
    box-sizing:border-box;
    width:inherit;
    height:100vh;
  }
  .blureffect{
    backdrop-filter:blur(15px);
  }
  .modalActive{
    display:flex;
    justify-content:center;
    align-items:center;
  }

  .content-modal{
    box-sizing:border-box;
    padding: 1rem 1rem;
    width:100%;
    background-color:#3f4d5a;
    border-radius:10px;
  }
  .header-modal{
    display:flex;
  }
  .btn-closed{
    margin-left:auto;
    width:2.3rem;
    color:#c00;
    background-color:none;
  }
  .btn-closed:hover{
    color:#f00;
  }
  @media (min-width: 650px){
    .content-modal{
      width:650px;
    }
  }
</style>

<container class:modalActive class:blureffect>
  <div class="content-modal">
    <div class="header-modal">
      <h2>Suscribete!</h2>
      <div class="btn-closed" on:click={modalHandler}>
        <GoX></GoX>
      </div>
    </div>
    <h1>hola</h1>
  </div>
</container>
