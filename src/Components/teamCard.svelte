<script>

  export let picture;
  export let name;
  export let title;
  export let gitHubLink;
  export let linkedInLink;
  import gitHubLogo from '../../assets/githubTransparent.png';
  import linkedInTransparent from '../../assets/linkedInTransparent.png';

</script>

<style type='text/scss'>

  @import '../styles.scss';
</style> 

<div id='teamCard'>
  <div id='nameTitle'>
    <h2>{name}</h2>
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


