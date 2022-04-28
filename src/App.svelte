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


<style lang='scss'>

	$navbarSize: 50px; 

#app{
	display: flex;
	flex-direction: column;
	align-items: center;
	justify-content: center;
	padding-top: $navbarSize;

	width: 100%;
}
</style>