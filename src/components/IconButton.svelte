<script>
  export let url= "https://luispfcanales.ga"
  export let ToLeft = false;
</script>

<a class:ToLeft href={url} target="_blank">
  <slot></slot>
</a>
<style>
  a{
    display:inline-block;
    color:#bbb;
    width:2rem;
    transition:.4s;
  }
  a:hover{
    color:#fff;
  }
  .ToLeft{
    margin-left: auto;
  }
</style>

