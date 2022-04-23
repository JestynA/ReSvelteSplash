


<div id='banner'>
    <h1>ReSvelte</h1>
    <div id='description'>
        VS Code Extension developer tool for
        Svelte application components
    </div>
    <div id='buttonsContainer'>
        <a href='https://github.com/oslabs-beta/ReSvelte'>
            <button>
                Contribute
            </button>
        </a>
        <a href='https://careers.mcdonalds.com/country'>
            <button>
                Install
            </button>
        </a>
    </div>



</div>




<style lang='scss'>

h1{
    font-size: 600%;
    animation: fadeInFromLeft 4s;
    margin-bottom: 20px;
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

#buttonsContainer{
    display: flex;
    gap: 20px;
    animation: fadeIn 4s;
    margin-top: 20px;
}

#description{
    margin: 0px 0px 20px 0px;
    animation: fadeIn 4s;
}

button{
    width: 15vw;
    height: 100%
}

button:hover{
    filter: brightness(80%)
}

#banner{
    padding: 100px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;

    div{
        width: 50%;
        display: flex;
        justify-content: center;
    }
}
</style>