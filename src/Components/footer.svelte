<script>
  import githubLogo from '../../assets/githubTransparent.png'
  import linkedinLogo from '../../assets/linkedInTransparent.png'
</script>

<style type='text/scss'>

  @import '../styles.scss';

</style>

<div id='footer'>

  <div class='column'>
    <h2>Contact us</h2>
    <div>Email: <a href='mailto:resvelteadm@gmail.com'>resvelteadm@gmail.com</a></div>
    
  </div>
  <div class='column' id='linksColumn'>
    <h2 id='links'>Links</h2>
    <div class='picLine'><img src={githubLogo} alt='gitHubLogo'/><a href='https://github.com/oslabs-beta/ReSvelte'>Github</a></div>
    <div class='picLine'><img src={linkedinLogo} alt='linkedInLogo'/><a href='https://www.linkedin.com/company/resvelte'>LinkedIn</a></div>
    
  </div>

</div>


