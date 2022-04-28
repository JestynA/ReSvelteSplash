<script>
  import TeamCard from "./teamCard.svelte";

  import candiePic from '../../assets/teamPics/Candie.png';
  import hoonPic from '../../assets/teamPics/Hoon.jpg';
  import jestynPic from '../../assets/teamPics/Jestyn.jpg';
  import martinPic from '../../assets/teamPics/Martin.jpg';
  import stevenPic from '../../assets/teamPics/Steven.jpg';

</script>

<style type='text/scss'>

  @import '../styles.scss';

</style>

<div id='teamContainer'>
  <div>
    <h1>The Team</h1>
  </div>
  <div id='cardContainer'>
    <TeamCard 
    name={'Candie Hill'} 
    picture={candiePic} 
    title='Software Engineer'
    gitHubLink='https://github.com/can619'
    linkedInLink='https://www.linkedin.com/in/candie-hill/'
    />

    <TeamCard 
    name='Hoon Park' 
    picture={hoonPic} 
    title='Software Engineer'
    gitHubLink='https://github.com/hoonpvrk'
    linkedInLink='https://www.linkedin.com/in/hoonpvrk'
    />

    <TeamCard 
    name='Jestyn Apuya' 
    picture={jestynPic} 
    title='Software Engineer'
    gitHubLink='https://github.com/JestynA'
    linkedInLink='https://www.linkedin.com/in/jestynapuya/'
    />

    <TeamCard 
    name='Martin Ng' 
    picture={martinPic} 
    title='Software Engineer'
    gitHubLink='https://github.com/kamartinng'
    linkedInLink='https://www.linkedin.com/in/martinngsf'
    />

    <TeamCard 
    name='Steven Nguyen'
    picture={stevenPic} 
    title='Software Engineer'
    gitHubLink='https://github.com/Sateeven'
    linkedInLink='https://www.linkedin.com/in/nguyennsteven'
    />
    
  </div>
</div>





