<script>
    import importGif from '../../assets/importGif.gif'
    import treeGif from '../../assets/treeGif.gif'
    import errorGif from '../../assets/errorGif.gif'
</script>


<div id='featuresContainer'>


    <div id='importingDemo' class='feature'>

        <div id='importGif'>
            <img src={importGif} />
        </div>

        <div id='importDesc' class='featureDesc'>
            <h2>Import your svelte project directly into VS Code</h2>
            <p>Work on your project and use ReSvelte simultaneously</p>
            
        </div>
    </div>

    <div id='componentTreeDemo' class='feature'>

        <div id='treeDesc' class='featureDesc'>
            <h2>Visualize your Svelte application</h2>
            <p>The component tree assists in debugging rerendering components.</p>
             
        </div>


        <div id='treeGif'>
            <img src={treeGif} />
        </div>


    </div>

    <div id='performanceMetricsDemo' class='feature'>
        <div id='performanceGif'>
            <img src={errorGif} />
        </div>
        <div id='performanceDesc' class='featureDesc'>
            <h2>Analyze your application</h2>
            <p>App Performance displays live data of your project</p>
        </div>
    </div>
</div>

<style lang='scss'>
    $descriptionCardColor: rgb(54,57,63);
    $backgroundColor: rgb(32,34,37);
    $fontColor: rgb(219,214,207);

    #featuresContainer{
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        gap: 10vh;


        margin: 0px 10% 0px 10%;
        padding: 150px 0px 150px 0px;
        width: 100%;
        
        box-shadow: 0px 0px 20px black;
        background-color: $backgroundColor;

        #importingDemo{
            opacity: 0;
            animation: fadeInFromLeft 2s 1s forwards;
        }
        #componentTreeDemo{
            opacity: 0;
            animation: fadeInFromRight 2s 1.5s forwards;
        }
        #performanceMetricsDemo{
            opacity: 0;
            animation: fadeInFromLeft 2s 2s forwards;
        }


        p{
            font-size: 70%;
            font-weight: lighter;
        }

        .feature{
        display: flex;
        justify-content: center;
        gap: 250px;
        align-items: center;
        width: 100%;
    }

    .featureDesc{

        text-align: left;


        font-size: 200%;
        
        padding: 0px 20px 0px 20px;
        width: 20%;
        height: 400px;

        
        //background-color: $descriptionCardColor;

        color: $fontColor;
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