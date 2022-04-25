<script>

  export let picture;
  export let name;
  export let title;
  export let gitHubLink;
  export let linkedInLink;
  import gitHubLogo from '../../assets/githubTransparent.png';
  import linkedInTransparent from '../../assets/linkedInTransparent.png';

</script>


<div id='teamCard'>
  <div id='nameTitle'>
    <h3>{name}</h3>
    <h4>{title}</h4>
  </div>

  <div id='pic'>
    <img src={picture} id='profilePic'/>
  </div>

  <div id='links'>

    <div id='gitHub'>
      <a href={gitHubLink}>
        <img src={gitHubLogo} alt='Image Error' class='logos'/>
      </a>
    </div>

    <div id='linkedIn'>
      <a href={linkedInLink}>
        <img src={linkedInTransparent} alt='Image Error' class='logos'/>
      </a>
    </div>

  </div>

</div>

<style lang='scss'>

  $cardColor: rgb(32,34,37);
  $fontColor: rgb(219,214,207);

  #profilePic{
    height: 80%;
    object-fit: contain;

    border-radius: 50%;
    border-style: sold;
    border-color: black;
  
  }

  .logos{
    height: 70px;
    width: 70px;
    
    object-fit: contain;
  }

  a{
    height: 100%;
    width: 100%;
  
  }

#teamCard{
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  height: 550px;
  width: 400px;

  background-color: $cardColor;
  border-radius: 20px;
  padding: 20px 0px 20px 0px;

  box-shadow: 0px 0px 15px rgb(24, 24, 24);

  h3,h4{
    margin: 0;
  }

  h4{
    font-weight: normal;
  }


  #nameTitle{
    display: flex;
    flex-direction: column;
    align-items: center;
    color: $fontColor;
    height: 10%;
  }

  #pic{
    display: flex;
    justify-content: center;
    align-items: center;
    height: 60%;
  }

  #links{
    width: 100%;
    display: flex;
    justify-content: space-around;
    height: 10%;
  }




}

</style> 