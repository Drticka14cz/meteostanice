<main><nav class="navigace"><div class="navigace_div"><a class="logo_nav" href="/"><img src="logo_meteostanice.png" alt="logo meteostanice navigace" id="logo_nav_id" ></a></div>
    <div class="navigace_div navigace_div_text"><a class="navigace_div_text_text" href="/">DOMŮ</a></div>
    <div class="navigace_div navigace_div_text"><a class="navigace_div_text_text" href="/navody">NÁVODY</a></div>
    <div class="navigace_div navigace_div_text"><a class="navigace_div_text_text" href="/dokumenty">VÝVOJ</a></div></nav>
<div class="mid"><h1>Vývoj Meteostanice</h1>
Začátek projektu na hardware započal v lednu roku 2026. Původní návrh nebyl ani blízko meteostanici. Prvnotní návrh byl gameboy, nebo nějaká malá kompaktní herní konzole. Avšak po rozhovoru s vedoucím práce, panem ing. L. Jacečkem jsme došli k tomu, že zkusíme něco jiného. Hlavním problémem by byl totiž samotný display. 
<p>Později po několika nápadech a hledání na <a href="https://dratek.cz/">drátek.cz</a> jsme se rozhodli udělat meteostanici. Hlavní součástka je <a href="https://dratek.cz/arduino-platforma/1361-bme280-modul-mereni-teploty-vlhkosti-a-barometrickeho-tlaku-precizni.html">modul meteočidla BMP280 3v1</a>. Dále používáme LCD display, tlačítka a rgb led. Více o tom co se nachází v meteostanici najdete na návodech <a href="/navody">zde</a>. </p>
<p class="uprostred">Jeden z prvních návhrhů vypadal takto:</p><img src="kapka.png" alt="prvni_navrh" class="">

</div></main>

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
        padding: 5% 15% 5% 15%;
    }
    h1{
        text-align: center;
        font-family: var(--font-mono);
        margin-bottom: 1rem;
    }
    .uprostred{
        text-align: center;
       
    
    }
    
</style>