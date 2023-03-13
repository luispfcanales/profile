<script>
  export let text = "mantenible...";

</script>
  <span
    style={`width:${text.length}ch;`}>
    {text}
  </span>

<style>
  span{
    display:inline-block;
    color:#bababa;
    font-size: 4rem;
    font-family: monospace;
    white-space:nowrap;
    display:inline-block;
    color:#f2c150;
    border-right:3px solid #f2c150;
    animation: 
      typing 3s infinite steps(35) alternate,
      blink .5s infinite step-end alternate;
    overflow:hidden;
  }
  @keyframes typing {
  from { width:0}
  }

  @keyframes blink {
  50%{ border-color: transparent; }
  }

@media (max-width:1024px){
  span{
    font-size: 2.4rem;
  }
}
</style>
