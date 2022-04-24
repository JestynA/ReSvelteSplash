<script>


import logo from '../../assets/ReSvelte.png'

</script>


<div id='navBar'>
    <div id='logo'><img src={logo} /></div>
    <div id='navButtons'>
        <button><div class='buttons'>Features</div></button>
        <button><div class='buttons'>Contribute</div></button>
        <button><div class='buttons'>The Team</div></button>
        
        

    </div>

</div>


<style lang='scss'>

$navbarSize : 50px;
$navbarColor: rgb(32,34,37);
$fontColor: rgb(163,166,170);

#navBar{
    display:flex;
    flex-direction: row;
    justify-content: space-between;
    background-color: $navbarColor;
    height: $navbarSize;
   
    position: fixed;
    top: 0; 
    width: 100%;
    
 

    div{
        height: 100%;
    }

    #logo{
        height: 100%;
           img{
        max-height: 100%;
    } 
    }

    #navButtons{
        display: flex;
        padding-right: 20px;
        
        button{
            padding-left: 20px;
            padding-right: 20px;
            height: 100%;
            background-color: $navbarColor;
            border-style: none;
        }

        button:hover{
            filter: brightness(70%)
        }
        .buttons{
            display: flex;
            align-items: center;
            color: $fontColor;
        }
    }


}




</style>