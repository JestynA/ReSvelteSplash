<script>

  import githubLogo from '../../assets/githubTransparent.png'
  import linkedinLogo from '../../assets/linkedInTransparent.png'
</script>

<div id='footer'>

  <div class='column'>
    <h2>Contact us</h2>
    <div>Email: <a href='mailto:resvelteadm@gmail.com'>resvelteadm@gmail.com</a></div>
    <div>Phone: <a href='tel:+14255058368'> Call/Text us here!</a></div>
    
  </div>
  <div class='column'>
    <h2 id='links'>Links</h2>
    <div class='picLine'><img src={githubLogo}/><a href='https://github.com/oslabs-beta/ReSvelte'>Github</a></div>
    <div class='picLine'><img src={linkedinLogo}/><a href='https://www.linkedin.com/company/resvelte'>LinkedIn</a></div>
    
  </div>

</div>


<style lang='scss'>
  $navbarColor: rgb(32,34,37);
  $fontColor: rgb(163,166,170);

  #footer{
    display: flex;
    justify-content: space-around;
    align-items: center;
    background-color: $navbarColor;
    padding: 10px 0px 100px 0px;
    width: 100%;
    box-shadow: 0px 0px 10px black;
    color: $fontColor;

    .column{
      display: flex;
      flex-direction: column;
      align-items: flex-start;
      gap: 20px;
      height: 80%;

      

    }

    .picLine{
      display: flex;
      align-items: center;
      gap: 10px;
      height: 50px;
    }

    img{
      height: 50%;
      width: 50%;
      object-fit: contain;
    }
  }

a{
  color: $fontColor;
}
</style>