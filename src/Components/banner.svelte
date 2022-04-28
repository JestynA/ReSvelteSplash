<script>

    import gitHub from '../../assets/githubTransparent.png'
    
</script>

<div id='banner'>
    <h1><span id='Re'>Re</span><span id='Svelte'>Svelte</span></h1>
    <div id='description'>
        <h2>VS Code Extension developer tool for
        Svelte applications</h2>
        
    </div>
    <div id='buttonsContainer'>
        
        <div id='contributeButton'>
            <button >
                <a href='https://github.com/oslabs-beta/ReSvelte' id='contributeButtonDisplay'>
                        <h2>Contribute</h2>
                </a> 
            </button>
        </div>

        <div id='installButton'>
            <button>
                <a href='https://marketplace.visualstudio.com/items?itemName=ReSvelte.resvelte' >              
                        <h2>Install</h2>               
                </a>
            </button>
        </div>

    </div>



</div>



<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Kanit:ital@1&display=swap" rel="stylesheet">
<style lang='scss'>

    $navbarSize: 100px;

    $primaryColor: rgb(147,213,232);
    $secondaryColor: rgb(59,104,195);
    $fontColor: rgb(163,166,170);

    $buttonColor: rgb(22,24,27);
    $buttonBorder: rgb(32,34,37);

img{
    height: 80%;
    object-fit: contain;
}

h1{
    font-family: 'Kanit', sans-serif;
    font-size: 1000%;
    font-weight: normal;
    animation: fadeInFromLeft 3s;
    margin-bottom: 20px;
    
    #Re{
        
        color: $primaryColor;
    }
    #Svelte{
        color: $secondaryColor;
    }
    
}

button{
    display: flex;
    align-items: center;
    height: 100%;
    width: 100%;
    min-width: fit-content;
    margin: 0;
    background-color: $buttonColor;
    border-color: $buttonBorder;
    border-style: solid;
    border-radius: 30px;


}

button:hover{
    filter: brightness(80%);
}




#buttonsContainer{
  
    display: flex;
    gap: 10vw;
    justify-content: center;
    animation: fadeIn 4s;

    height: 75px;

    #contributeButton{
        width: 20%;
    }

    #installButton{
        width: 20%;
    }
}

#description{

    color: $fontColor;

    margin: 0px 0px 50px 0px;
    animation: fadeIn 4s;
}





#banner{
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    width: 100%;
    background: linear-gradient(137deg, rgba(48,51,57,1) 0%, rgba(32,34,37,1) 55%);
    padding-bottom: 5%;


    div{
        width: 50%;
        display: flex;
        justify-content: center;
    }



    a{
        
        display: flex;
        justify-content: center;
        align-items: center;
        width: 100%;
        height: 100%;
        padding-left: 20px;
        padding-right: 20px;
        color: $fontColor;
        font-weight: bold;
        text-decoration: none;
    }
    a:hover{
        text-decoration: none;
    }

    
}

@keyframes fadeInFromLeft{
    0%{
        opacity: 0;
        transform: translateX(-150px);
    }
    100%{
        transform: translateX(0);
        opacity: 1;
    }
}

@keyframes fadeIn{
    0%{
        opacity: 0;
    }
    100%{
        opacity: 1;
    }
}

@media only screen and (max-width: 600px) {
  body {
    background-color: whitesmoke;
  }
}
</style>