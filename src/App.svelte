<script>
	import NavBar from './Components/navbar.svelte'
	import Banner from './Components/banner.svelte'
	import FeaturesContainer from './Components/featuresContainer.svelte'
	import TeamContainer from './Components/teamContainer.svelte'
	import Footer from './Components/footer.svelte';


</script>

<div id='app'>
	<NavBar/>
	<Banner/>
	<FeaturesContainer/>
	<TeamContainer/>
	<Footer/>
</div>


<style type='text/scss'>
@import './styles.scss';
</style>