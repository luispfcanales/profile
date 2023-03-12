<div>
  <span>Sube de nivel.</span>
  <span>Haz código</span>
  <slot></slot>
</div>

<style>
  span{
    display:inline-block;
    color:#bababa;
    font-size: 4rem;
    font-family: monospace;
    white-space:nowrap;
  }
  div{
    margin:0;
    padding:0;
    box-sizing:border-box;
    display:flex;
    flex-direction:column;
  }
  
@media (max-width:800px){
  div{
    align-items:center;
  }
  span{
    font-size: 2.4rem;
  }
}
</style>
