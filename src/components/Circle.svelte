<script>
  let positionX = 30;
  const slowMin = 15;
  const slowMax = 45;
  function ChangeX() {
    positionX = Math.floor(Math.random() * 1550)
    return positionX
  }
  function GetNumberSlow(){
    return Math.floor(Math.random() * ( slowMax - slowMin + 1) + slowMin)
  }
</script>

<span style={`left:${ChangeX()}px;--i:${GetNumberSlow()}`}></span>
<span style={`left:${ChangeX()}px;--i:${GetNumberSlow()}`}></span>
<span style={`left:${ChangeX()}px;--i:${GetNumberSlow()}`}></span>
<span style={`left:${ChangeX()}px;--i:${GetNumberSlow()}`}></span>
<span style={`left:${ChangeX()}px;--i:${GetNumberSlow()}`}></span>
<span style={`left:${ChangeX()}px;--i:${GetNumberSlow()}`}></span>
<span style={`left:${ChangeX()}px;--i:${GetNumberSlow()}`}></span>
<span style={`left:${ChangeX()}px;--i:${GetNumberSlow()}`}></span>
<span style={`left:${ChangeX()}px;--i:${GetNumberSlow()}`}></span>
<span style={`left:${ChangeX()}px;--i:${GetNumberSlow()}`}></span>
<span style={`left:${ChangeX()}px;--i:${GetNumberSlow()}`}></span>
<span style={`left:${ChangeX()}px;--i:${GetNumberSlow()}`}></span>
<span style={`left:${ChangeX()}px;--i:${GetNumberSlow()}`}></span>
<span style={`left:${ChangeX()}px;--i:${GetNumberSlow()}`}></span>
<span style={`left:${ChangeX()}px;--i:${GetNumberSlow()}`}></span>
<span style={`left:${ChangeX()}px;--i:${GetNumberSlow()}`}></span>
<span style={`left:${ChangeX()}px;--i:${GetNumberSlow()}`}></span>
<span style={`left:${ChangeX()}px;--i:${GetNumberSlow()}`}></span>
<span style={`left:${ChangeX()}px;--i:${GetNumberSlow()}`}></span>
<span style={`left:${ChangeX()}px;--i:${GetNumberSlow()}`}></span>
<span style={`left:${ChangeX()}px;--i:${GetNumberSlow()}`}></span>
<span style={`left:${ChangeX()}px;--i:${GetNumberSlow()}`}></span>
<span style={`left:${ChangeX()}px;--i:${GetNumberSlow()}`}></span>
<span style={`left:${ChangeX()}px;--i:${GetNumberSlow()}`}></span>
<span style={`left:${ChangeX()}px;--i:${GetNumberSlow()}`}></span>
<span style={`left:${ChangeX()}px;--i:${GetNumberSlow()}`}></span>
<span style={`left:${ChangeX()}px;--i:${GetNumberSlow()}`}></span>
<span style={`left:${ChangeX()}px;--i:${GetNumberSlow()}`}></span>
<span style={`left:${ChangeX()}px;--i:${GetNumberSlow()}`}></span>
<span style={`left:${ChangeX()}px;--i:${GetNumberSlow()}`}></span>
<span style={`left:${ChangeX()}px;--i:${GetNumberSlow()}`}></span>

<style>
  span{
    position:absolute;
    width:25px;
    height:25px;
    background:var(--bg-color-circle);
    border-radius:50%;
    box-shadow: 0 0 7px var(--bg-color-circle-shadow),
      0 0 10px var(--bg-color-circle-shadow),
      0 0 15px var(--bg-color-circle-shadow);
    top:-10px;
    animation:move-circle 15s linear infinite;
    animation-duration:calc(125s / var(--i));
  }
  span:nth-child(even){
    background:var(--bg-color-circle2);
    box-shadow: 0 0 7px var(--bg-color-circle2-shadow),
      0 0 10px var(--bg-color-circle2-shadow),
      0 0 15px var(--bg-color-circle2-shadow);
  }
  @keyframes move-circle {
  0%{
    transform:translateY(100vh) scale(0);
  }
  100%{
    transform:translateY(-10vh) scale(1);
  }
  }
</style>
