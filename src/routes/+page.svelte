<div class="main">
    <div class="uvod"><div class="uvod_logo"><img src="logo_meteostanice.png" alt="logo meoteostanice" id="logo_meteostanice"></div><div class="uvod_pointer"><a href="#nav"><img src="pointer_2.svg" alt="pointer_2.svg" id="pointer"></a></div></div>
    <div class="mid"><nav class="navigace" id="nav"><div class="navigace_div"><a class="logo_nav" href="/"><img src="logo_meteostanice.png" alt="logo meteostanice navigace" id="logo_nav_id" ></a></div>
    <div class="navigace_div navigace_div_text"><a class="navigace_div_text_text" href="/">DOMŮ</a></div>
    <div class="navigace_div navigace_div_text"><a class="navigace_div_text_text" href="/navody">NÁVODY</a></div>
    <div class="navigace_div navigace_div_text"><a class="navigace_div_text_text" href="/dokumenty">VÝVOJ</a></div></nav>


meteo</div>
    
</div>
<style>
    .uvod {
    background-image: url("/meteo_pozadi.png");
    background-size: cover;
    background-repeat: repeat-x;
    background-position: 0 0;
    height: 100vh;
    width: 100%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    gap: 10vh;
    /* padding-top:10vh; */
    align-items: center;
    animation: posun 30s linear infinite;
    background-color: rgb(29, 113, 184);
}

@keyframes posun {
    from {
        background-position:0;
    }
    to {
        background-position:100vw ;
    }
}

    .uvod_logo{
        height: 40%;
        width: 40%;
        /* border: red dashed 2px; */
        display: flex;
        justify-content: center;
        align-items: center;
        align-content: center;

    }
    .uvod_logo img{
        transition: transform 1s linear;
        display: inline-block;
    }
    .uvod_logo img:hover{
        transform: scale(1.2) translateX(1rem) translateY(1rem) rotate(-3deg);
        animation: logo_mrak infinite 10s ease alternate;
    }
    @keyframes logo_mrak{
        0%{
            transform: translateX(0vw) translateY(0vh) rotate(0deg);
            
        }
        25%{
            transform: translateX(1vw) translateY(-0.5vh) rotate(4deg);
            
        }
        50%{
            transform: translateX(-0.5vw) translateY(2vh) rotate(0deg) scale(1.1);
            
        }
        75%{
            transform: translateX(-1vw) translateY(-0.5vh) rotate(-3deg)scale(0.9);
            
        }
        100%{
             transform: translateX(0vw) translateY(0vh) rotate(2deg) ;

        }
    }
    #logo_meteostanice{
        height: 100%;
        margin-top: 25vh;
      
    }
    .uvod_pointer{
        /* border: red dashed 5px; */
        width: 8vw;
        height: 8vh;
        padding-top: 20vh;
        /* filter: opacity(60%); */
        
filter: brightness(0) saturate(100%) invert(38%) sepia(17%) saturate(0%) hue-rotate(178deg) brightness(101%) contrast(98%);
    }
    #pointer{
        max-width: 100%;
        min-width: 100%;
        animation: pointer_ani alternate infinite 5s ease-in-out;
        
        

    }
    @keyframes pointer_ani{
        0%{
            transform: translateY(-8%);
        }
        15%{
            transform: translateY(25%);
        }
        30%{
            transform: translateY(-5%);
         }
         45%{
            transform: translateY(25%);

         }
         60%{
            transform: translateY(-5%);
         }
         75%{
            transform: translateY(0%);
         }
         100%{
            transform: translateY(0%);
         }
    }

    .logo_nav{
        text-decoration: none;
        transition: transform 1s ease;
        display: inline-block;
    }
    #logo_nav_id{
        max-height:9vh;
    }
    .logo_nav:hover{
        transform: scale(1.1) rotate(-0deg) translateX(0.2rem) translateY(0.1rem);
    }

    .navigace{
        max-width: 100%;

        height: 10%;
        border-top: 0.5vh rgb(16, 64, 102) solid;
        position: sticky;
        top: 0;
        display: flex;
        flex-direction: row;
        gap: 10%;
        background-color: rgba(178, 178, 178, 0.2) ;
        padding-right: 10vw;
        font: var(--font-mono);
        font-weight: 500;
        font-size: larger;
        
        
    }
    .navigace_div{
        /* border: red dashed 1px; */
        /* width: 50%;
        max-width: 100%; */
        flex: 1;
    }
    .navigace_div_text{
        text-align: center;
        align-content: center;
        border-radius: 0% 0% 50% 50%;
        transition: background-color 0.9s ease;
        background-color: none;
        padding: 2%;
    }
    .navigace_div_text:hover{
        background-color:  rgba(29, 113, 184, 0.8);
        
    }
    .navigace_div_text a{
        text-decoration: none;
        transition: transform 0.5s ease;
        display: inline-block;
        color: inherit;
        text-decoration: none;
    }
    .navigace_div_text a:hover{
        transform: scale(1.2) translateY(-0.3rem) rotate(2deg);
        
        
    }
    .mid{
        min-height: 100vh;
    }


</style>