<script>
  export let text = "primary"
  export let modalHandler;
</script>
<button on:click={modalHandler}>
{text} 
</button>
<style>
  button{
    margin:0;
    margin-top: 2.6rem;
    padding:8px 0;
    display:flex;
    justify-content:center;
    gap:10px;
    min-width:310px;
    max-width:360px;
    background-color:var(--bg-body-color);
    color:#f08f90;
    font-size:2rem;
    border:2px solid #f08f90;
    border-radius: 10px;
    transition:.5s;
  }
  button:hover{
    background-color:#f08f90;
    color:var(--bg-body-color);
  } 
  </style>
