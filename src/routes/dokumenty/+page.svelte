<main><nav class="navigace" id="nav"><div class="navigace_div"><a class="logo_nav" href="/"><img src="logo_meteostanice.png" alt="logo meteostanice navigace" id="logo_nav_id" ></a></div>
    <div class="navigace_div navigace_div_text"><a class="navigace_div_text_text " href="/">DOMŮ</a></div>
    <div class="navigace_div navigace_div_text"><a class="navigace_div_text_text " href="/navody">NÁVODY</a></div>
    <div class="navigace_div navigace_div_text"><a class="navigace_div_text_text" href="/dokumenty">VÝVOJ</a></div></nav>
<div class="mid"><h1>Vývoj Meteostanice</h1>
Začátek projektu na hardware započal v lednu roku 2026. Původní návrh nebyl ani blízko meteostanici. Prvnotní návrh byl gameboy, nebo nějaká malá kompaktní herní konzole. Avšak po rozhovoru s vedoucím práce, panem ing. L. Jacečkem jsme došli k tomu, že zkusíme něco jiného. Hlavním problémem by byl totiž samotný display. 
<p>Později po několika nápadech a hledání na <a href="https://dratek.cz/">drátek.cz</a> jsme se rozhodli udělat meteostanici. Hlavní součástka je <a href="https://dratek.cz/arduino-platforma/1361-bme280-modul-mereni-teploty-vlhkosti-a-barometrickeho-tlaku-precizni.html">modul meteočidla BMP280 3v1</a>. Dále používáme LCD display, tlačítka a rgb led. Více o tom co se nachází v meteostanici najdete na návodech <a href="/navody">zde</a>. </p>
<p class="uprostred">Jeden z prvních návhrhů vypadal takto:</p><div class="uprostred"><img src="navrh_meteostanice_1.png" alt="prvni_navrh" class="obrazek_1"></div>
<p>Následně jsme se pustili do návrhu kompletního vzhledu brandu. Tomáš udělal brand manuál, dle kterého jsme navrhli tento web, propagační leták i samotnou meteostanici. Hlavním prvkem je žluté slunce, bílý mrak a další grafické prvky. Vše je kombinováno do pár barev, které jsou vidět na tomto webu.</p>
<div class="ukazka_disegnu_div"> <img src="logo_meteostanice.png" alt="logo" class="disegn"><img src="kapka.png" alt="kapka" class="disegn"><img src="teplota.png" alt="teplota" class="disegn"></div>
<p>Následně Kuba udělal zapojení v tinkercadu a po čekání na komponenty bylo zapojení i kód otestováno fyzicky. Avšak bylo to nefunkční - některé komponenty chtěly jiný kód. Následně vše bylo fixnuto a mozek Meteostanice již fungoval.</p>
<div class="uprostred"><img src="Meteostanice_zapojeni.png" alt="vzhled zapojení" class="obrazek_1 rotate"></div>
<p>Během utrpení při zapojování a psaní kódu pro arduino tak Tomáš pracoval na 3D modelu. Vše bylo vyměřeno přímo na komponenty meteostanice a tak vznikla unikátní krabička naší meteostanice. 3D model byl vypracován v nejlepším programu na 3D modely - Solid works. Během tvorby nebyl žádný problém :D. </p>
<div class="uprostred ukazka_disegnu_div"><img src="meteostanice_solidSCR_1.png" alt="screen z solidu" class="obrazek_1 disegn"><img src="meteostanice_solidSCR_2.png" alt="druhy screen ze solidu" class="obrazek_1 disegn"></div>

<p id="obsah">Finální obsah projektu:</p>


</div></main>

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
        z-index: 100;
        
        
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

@media (max-width: 768px){
    .navigace {
        flex-wrap: nowrap; /* Zabráníme zbytečnému skákání na 100 řádků */
        flex-direction: row; 
        justify-content: space-around; /* Rozprostře položky vedle sebe */
        height: auto; 
        padding: 10px 0; /* Minimální padding */
        gap: 0;
    }

    .navigace_div {
        width: auto; /* Zrušeno 100%, aby nebyly pod sebou jako obří bloky */
        flex: 1;
        display: flex;
        justify-content: center;
        align-items: center;
    }

    .navigace_div_text_text {
        padding: 10px 5px; /* Menší vnitřní prostor na mobilu */
        font-size: 0.9rem; /* Trochu menší písmo, aby se to vešlo */
        display: flex;
        justify-content: center;
        align-items: center;
    }

    .navigace_div_text {
        border-radius: 5px; /* Méně agresivní zaoblení na mobilu */
    }

    #logo_nav_id {
        max-height: 5vh; /* Menší logo v liště */
    }

    /* Oprava textových sekcí na mobilu, aby nebyly tak nalepené na kraje */
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
    .ukazka_disegnu_div{
        display: flex;
        flex-wrap: wrap;
        flex-direction: row;
        justify-content: center;
        gap: 15%  ;
    }
    .disegn{
        height: 10rem;
        width: auto;
        margin-top: 5%;
        margin-bottom: 10%;

    }
    .obrazek_1{
        height: 40%;
        width: 40%;
        margin: 2% 0 7% 0;

    }
    .rotate{
        transform: rotate(90deg);
    
    }
    @media (max-width:768px){
        .obrazek_1{
            height: 75%;
            width: 75%;
        }
    }
    
</style>