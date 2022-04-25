<script>

    import gitHub from '../../assets/githubTransparent.png'
    
</script>



<div id='banner'>
    <h1><span id='Re'>Re</span><span id='Svelte'>Svelte</span></h1>
    <div id='description'>
        VS Code Extension developer tool for
        Svelte application components
    </div>
    <div id='buttonsContainer'>
        
        <div id='contributeButton'>
            <button >
                <a href='https://github.com/oslabs-beta/ReSvelte' id='contributeButtonDisplay'>
                        <img src={gitHub}/>  
                        Contribute
                </a> 
            </button>
        </div>

        <div id='installButton'>
            <button>
                <a href='https://careers.mcdonalds.com/country' >              
                        Install               
                </a>
            </button>
        </div>

    </div>



</div>



<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Kanit:ital@1&display=swap" rel="stylesheet">
<style lang='scss'>



    $primaryColor: rgb(147,213,232);
    $secondaryColor: rgb(59,104,195);
    $fontColor: rgb(163,166,170);

    $buttonColor: rgb(32,34,37);
    $buttonBorder: rgb(32,34,37);

img{
    height: 80%;
    object-fit: contain;
}

h1{
    font-family: 'Kanit', sans-serif;
    font-size: 600%;
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
    margin: 0;
    background-color: $buttonColor;
    border-color: $buttonBorder;
    border-style: solid;
    border-radius: 10px;


}

button:hover{
    filter: brightness(80%);
}




#buttonsContainer{
  
    display: flex;
    gap: 20px;
    justify-content: space-between;
    animation: fadeIn 4s;
    width: 25%;

    #contributeButton{
        width: 10%;
        height: 50px;
    }

    #installButton{
        width: 10%;
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
    padding-bottom: 50px;


    div{
        width: 50%;
        display: flex;
        justify-content: center;
    }

    #contributeButtonDisplay{
        display: flex;
        width: 100%;
        justify-content: space-between;
        padding-right: 5px;
    }

    a{
        
        display: flex;
        justify-content: center;
        align-items: center;
        width: 100%;
        height: 100%;
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
</style>