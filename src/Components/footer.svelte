

<div id='footer'>

  <div class='column'>
    Contact us <br/>
    <div>Email: <a href='mailto:resvelteadm@gmail.com'>resvelteadm@gmail.com</a></div>
    <div>Phone: <a href='tel:+14255058368'> Call/Text us here!</a></div>
    
  </div>
  <div class='column'>
    <a>HELLLOOO</a>
    <a>HELLLOOO</a>
    <a>HELLLOOO</a>
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
      align-items:center;
      gap: 20px;
    }
  }

a{
  color: $fontColor;
}
</style>