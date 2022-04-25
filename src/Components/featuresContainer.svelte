<script>
    import testGif from '../../assets/frenchieGif.gif'
</script>


<div id='featuresContainer'>


    <div id='importingDemo' class='feature'>

        <div id='importGif'>
            <img src={testGif} />
        </div>

        <div id='importDesc' class='featureDesc'>
            Import your svelte project directly into VS Code so you can 
            work on you project simultaneously!
        </div>
    </div>

    <div id='componentTreeDemo' class='feature'>

        <div id='treeDesc' class='featureDesc'>
            Visualize your Svelte application as a component tree 
            to help debug rerendering components.
        </div>


        <div id='treeGif'>
            <img src={testGif} />
        </div>


    </div>

    <div id='performanceMetricsDemo' class='feature'>
        <div id='performanceGif'>
            <img src={testGif} />
        </div>
        <div id='performanceDesc' class='featureDesc'>
            Analyze your application using the Performance Metrics.
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
            animation: fadeInFromLeft 4s 1s forwards;
        }
        #componentTreeDemo{
            opacity: 0;
            animation: fadeInFromRight 4s 2s forwards;
        }
        #performanceMetricsDemo{
            opacity: 0;
            animation: fadeInFromLeft 4s 3s forwards;
        }

            .feature{
        display: flex;
        justify-content: space-around;
        align-items: center;
        width: 100%;
    }

    .featureDesc{
        text-align: center;
        display: flex;
        align-items: center;
        padding: 0px 20px 0px 20px;
        width: 35%;
        height: 50%;
        background-color: $descriptionCardColor;
        border-radius: 20px;
        border-style: none;
        color: $fontColor
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