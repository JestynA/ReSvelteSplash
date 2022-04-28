<script>

    import logo from '../../assets/RSonly.png'
    
    </script>
    
    <div id='navBar'>
        <div id='logo'>
            <a href='#' id='logoButton'>
              <img src={logo} />  
            </a>   
        </div>
    
        <div id='navButtons'>
        <a href='#featuresContainer'><div class='buttons'>Features</div></a>
        <a href='https://github.com/oslabs-beta/ReSvelte'><div class='buttons'>Contribute</div></a>
        <a href='#teamContainer'><div class='buttons'>The Team</div></a>
            
            
            
        </div>
    </div>
    
    
    <style lang='scss'>
    
    $navbarSize : 70px;
    $navbarColor: rgb(32,34,37);
    $fontColor: rgb(163,166,170);
    
    #navBar{
        display:flex;
        flex-direction: row;
        background-color: $navbarColor;
        height: $navbarSize;
        position: fixed;
        top: 0; 
        width: 100%;
        box-shadow: 0px 0px 10px black;
        z-index: 9999;
     
        div{
            height: 100%;
        }
    
        #logo{
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            padding-left: 3vw;
            height: 100%;
            font-size: 1vw;
               img{
            max-height: 80%;
        } 
            #logoButton{
                display: flex;
                align-items: center;
                height: 100%;
                width: 100%;
                background-color: $navbarColor;
                border-style: none;
                padding: 0;
                margin: 0;
            }
    
            #logoButton:hover{
                cursor: pointer;
            }
        }
    
        #navButtons{
            display: flex;
            margin-left: auto;
            justify-content: space-around;
            width: 30%;
           
            a{
                height: 100%;
                font-size: 150%;
                text-decoration: none;
                background-color: $navbarColor;
                border-style: none;
                font-size: 1vw;
                width: 33%;
                display: flex;
                justify-content: center;
            }
    
            a:hover{
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