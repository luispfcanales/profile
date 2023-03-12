<script>
  export let text = "primary"
</script>
<button>
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
    width:90%;
    background-color:var(--bg-body-color);
    color:#f08f90;
    font-size:2.5rem;
    border:2px solid #f08f90;
    border-radius: 10px;
    transition:.5s;
  }
  button:hover{
    background-color:#f08f90;
    color:var(--bg-body-color);
  } 
  </style>
