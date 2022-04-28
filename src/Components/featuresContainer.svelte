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

 <style lang='scss'>
    $descriptionCardColor: rgb(54,57,63);
    $backgroundColor: rgb(32,34,37);
    $fontColor: rgb(219,214,207);


    img{
            //width: 50vw;
            width: 100%;
            object-fit: contain;
        }

    #featuresContainer{
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        
        gap: 100px;
        padding-top: 150px;
        padding-bottom: 150px;

        // margin: 0px 10% 0px 10%;
        // padding: 150px 0px 150px 0px;
        width: 100%;
        
        box-shadow: 0px 0px 20px black;
        background-color: $backgroundColor;

        #importingDemo{
            opacity: 0;
            animation: fadeInFromLeft 2s 1s forwards;
            width: 90%;
        }
        #componentTreeDemo{
            opacity: 0;
            animation: fadeInFromRight 2s 1.5s forwards;
            width: 90%;
        }
        #performanceMetricsDemo{
            opacity: 0;
            animation: fadeInFromLeft 2s 2s forwards;
            width: 90%;
        }

        .gif{
            width: 100%;
        }


        p{
            font-size: 70%;
            font-weight: lighter;
        }

        .feature{
        display: flex;
        justify-content: center;
        gap: 5%;
        align-items: center;
        width: 100%;
    }

    .featureDesc{

        text-align: left;
        font-size: 200%;
        padding: 0px 20px 0px 20px;
        //background-color: $descriptionCardColor;
        color: $fontColor;
        width: 100%;
        
    }
    }



    @keyframes fadeInFromLeft{
        0%{
            opacity: 0;
            transform: translateX(-500px);
        }

        30%{
            opacity: .2;
        }
        100%{
            opacity: 1;
            transform: translateX(0);
        }
    }

    @keyframes fadeInFromRight{
        0%{
            opacity: 0;
            transform: translateX(500px);
        }

        30%{
            opacity: .2;
        }

        100%{
            opacity: 1;
            transform: translateX(0);
        }
    }

</style> 