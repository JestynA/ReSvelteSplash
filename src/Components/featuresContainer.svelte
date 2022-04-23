<script>

    import logo from '../../assets/ReSvelte.png'
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
    $descriptionCardColor: gray;

    #featuresContainer{
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        margin: 0px 10% 0px 10%;
        gap: 10vh;

        #importingDemo{
            opacity: 0;
            animation: fadeInFromLeft 4s 2s forwards;
        }
        #componentTreeDemo{
            opacity: 0;
            animation: fadeInFromRight 4s 3s forwards;
        }
        #performanceMetricsDemo{
            opacity: 0;
            animation: fadeInFromLeft 4s 4s forwards;
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