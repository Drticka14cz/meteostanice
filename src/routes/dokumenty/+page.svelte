<main><nav class="navigace"><div class="navigace_div"><a class="logo_nav" href="/"><img src="logo_meteostanice.png" alt="logo meteostanice navigace" id="logo_nav_id" ></a></div>
    <div class="navigace_div navigace_div_text"><a class="navigace_div_text_text" href="/">DOMŮ</a></div>
    <div class="navigace_div navigace_div_text"><a class="navigace_div_text_text" href="/navody">NÁVODY</a></div>
    <div class="navigace_div navigace_div_text"><a class="navigace_div_text_text" href="/dokumenty">DOKUMENTY</a></div></nav>
<div class="mid"><h1>Dokumenty</h1></div></main>
<style>
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
        transition: background-color 0.5s ease;
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
    /* konec navigace */
    .mid{
        min-height: 100vh;
    }
</style>