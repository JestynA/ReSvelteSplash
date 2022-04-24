<script>

    import gitHub from '../../assets/githubTransparent.png'
</script>


<div id='banner'>
    <h1>ReSvelte</h1>
    <div id='description'>
        VS Code Extension developer tool for
        Svelte application components
    </div>
    <div id='buttonsContainer'>
        <div>
            <button >
                <a href='https://github.com/oslabs-beta/ReSvelte' class='buttons'>
                        <img src={gitHub}/>
                        Contribute
                </a> 
            </button>
        </div>

        <div>
            <button>
                <a href='https://careers.mcdonalds.com/country' class='buttons'>              
                        Install               
                </a>
            </button>
        </div>

    </div>



</div>




<style lang='scss'>

    $h1Color: rgb(228,63,69);
    $descColor: rgb(146,145,150);
    $buttonColor: rgb(205, 205, 205);
    $buttonBorder: rgb(120, 120, 120);

img{
    height: 100%;
    object-fit: contain;
}

h1{
    font-size: 600%;
    animation: fadeInFromLeft 4s;
    margin-bottom: 20px;
    color: $h1Color;
    
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
}

#description{

    color: $descColor;

    margin: 0px 0px 20px 0px;
    animation: fadeIn 4s;
}





#banner{
    padding: 100px 0px 100px 0px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    width: 100%;

    div{
        width: 50%;
        display: flex;
        justify-content: center;
    }

    .buttons{
        display: flex;
        height: 30px;
    }

    a{
        
        display: flex;
        justify-content: center;
        align-items: center;
        width: 100%;
        height: 100%;
        color: black;
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