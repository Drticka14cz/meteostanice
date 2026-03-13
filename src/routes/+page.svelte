<div class="main">
    <div class="uvod"><div class="uvod_logo"><img src="logo_meteostanice.png" alt="logo meoteostanice" id="logo_meteostanice"></div></div>
    <div class="mid"><nav class="navigace"><div class="navigace_div"><a class="logo_nav" href="/"><img src="logo_meteostanice.png" alt="logo meteostanice navigace" id="logo_nav_id" ></a></div>
    <div class="navigace_div navigace_div_text"><a class="navigace_div_text_text" href="/">DOMŮ</a></div>
    <div class="navigace_div navigace_div_text"><a class="navigace_div_text_text" href="/navody">NÁVODY</a></div>
    <div class="navigace_div navigace_div_text"><a class="navigace_div_text_text" href="/dokumenty">DOKUMENTY</a></div></nav>


<img src="slunce.png" alt="slunko" height="500px"></div>
    
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
        height: 40vh;
        width: 40vw;
        /* border: red dashed 2px; */

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
        height: 40vh;
      
    }
    .logo_nav{
        text-decoration: none;
        transition: transform 1s ease;
        display: inline-block;
    }
    #logo_nav_id{
        height: 8vh;
    }
    .logo_nav:hover{
        transform: scale(1.1) rotate(-0deg) translateX(0.2rem) translateY(0.1rem);
    }

    .navigace{
        max-width: 100%;

        height: 8vh;
        border-top: 0.5vh rgb(16, 64, 102) solid;
        position: sticky;
        top: 0;
        display: flex;
        flex-direction: row;
        gap: 10%;
        background-color: rgba(178, 178, 178, 0.2) ;
        padding-right: 20%;
        font: var(--font-mono);
        font-weight: 500;
        font-size: larger;
        
    }
    .navigace_div{
        /* border: red dashed 1px; */

        width: 50%;
    }
    .navigace_div_text{
        text-align: center;
        align-content: center;
        border-radius: 0% 0% 50% 50%;
        transition: background-color 0.9s ease;
        background-color: none;
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