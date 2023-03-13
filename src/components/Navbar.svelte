<script>
  import { FaGithub,FaTwitter } from "svelte-icons/fa";
  import IconButton from "./IconButton.svelte";

  const urlDomain = "https://"
  const nameDomain = "luispfcanales"
  const urlProfile={
    github: urlDomain+"github.com/"+nameDomain,
    twitter: urlDomain+"twitter.com/"+nameDomain
  }
</script>

<div>
  <p>GopherDev</p>
  <IconButton ToLeft={true} url={urlProfile.twitter}>
    <FaTwitter/>
  </IconButton>
  <IconButton url={urlProfile.github}>
    <FaGithub />
  </IconButton>
</div>

<style>
  div{
    margin:0;
    padding:0;
    padding-top:1.4rem;
    box-sizing:border-box;
    display:flex;
    align-items:center;
    gap:10px;
    width:100%;
  }
  p{
    color:#bababa;
    font-size:2rem;
    font-weight:bold;
    font-style:Arial;
  }
</style>
