<script>
    import importGif from '../../assets/importGif.gif'
    import treeGif from '../../assets/treeGif.gif'
    import errorGif from '../../assets/errorGif.gif'
</script>


<div id='featuresContainer'>

    <div id='importingDemo' class='feature'>

        <div id='importGif' class='gif'>
            <img src={importGif} alt='importGif'/>
        </div>

        <div class='featureDesc'>
            <h2>Import your Svelte project directly into VS Code</h2>
            <p>Work on your project and use ReSvelte simultaneously</p>
            
        </div>
    </div>

    <div id='componentTreeDemo' class='feature'>

        <div class='featureDesc'>
            <h2>Visualize your Svelte application</h2>
            <p>The component tree assists in debugging rerendering components</p>
             
        </div>

        <div id='treeGif' class='gif'>
            <img src={treeGif} alt='treeGif'/>
        </div>


    </div>

    <div id='performanceMetricsDemo' class='feature'>
        <div id='performanceGif' class='gif'>
            <img src={errorGif} alt='errorGif'/>
        </div>
        <div class='featureDesc'>
            <h2>Analyze your application</h2>
            <p>App Performance displays live data of your project</p>
        </div>
    </div>
</div>

 <style type='text/scss'>
    @import '../styles.scss';
</style> 