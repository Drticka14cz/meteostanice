<main><nav class="navigace"><div class="navigace_div"><a class="logo_nav" href="/"><img src="logo_meteostanice.png" alt="logo meteostanice navigace" id="logo_nav_id" ></a></div>
    <div class="navigace_div navigace_div_text"><a class="navigace_div_text_text" href="/">DOMŮ</a></div>
    <div class="navigace_div navigace_div_text"><a class="navigace_div_text_text" href="/navody">NÁVODY</a></div>
    <div class="navigace_div navigace_div_text"><a class="navigace_div_text_text" href="/dokumenty">VÝVOJ</a></div></nav>
<div class="mid"><h1>Návody</h1></div></main>
<style>
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
        background-color: rgba(178, 178, 178, 0.72) ;
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
        align-content: stretch;
        
        border-radius: 0% 0% 50% 50%;
        transition: background-color 0.9s ease;
        background-color: none;
        
    }
    .navigace_div_text:hover{
        background-color:  rgba(29, 113, 184, 0.8);
        
    }
    .navigace_div_text a{
        
        transition: transform 0.5s ease;
        
    }
    .navigace_div_text a:hover{
        transform: scale(1.2) translateY(-0.3rem) rotate(2deg);
        
        
    }
    .navigace_div_text_text {
    display: block;       
    width: 100%;
    height: 100%;
    align-items: center; 
    justify-content: center; 
    text-decoration: none;
    color: inherit;
   
    padding: 10% 0;
    
}
    /* konec navigace */
    .mid{
        min-height: 100vh;
        
    }
</style>