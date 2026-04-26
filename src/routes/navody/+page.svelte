<script>
  import { walk } from "svelte/compiler";

</script>
<main><nav class="navigace" id="nav"><div class="navigace_div"><a class="logo_nav" href="/"><img src="logo_meteostanice.png" alt="logo meteostanice navigace" id="logo_nav_id" ></a></div>
    <div class="navigace_div navigace_div_text"><a class="navigace_div_text_text " href="/">DOMŮ</a></div>
    <div class="navigace_div navigace_div_text"><a class="navigace_div_text_text " href="/navody">NÁVODY</a></div>
    <div class="navigace_div navigace_div_text"><a class="navigace_div_text_text" href="/dokumenty">VÝVOJ</a></div></nav>
<div class="mid"><h1>Návody</h1>
    <p>Vítejte v návodu k použití naší Meteostanice. Před použitím si přečtěte celý návod.
    </p>


    <div class="navod_template">
    <h2>Přední strana meteostanice</h2>
        <img src="Meteo_navod_1_text.png" alt="navod 1" class=" navod_img_temp">
        <div class="popisky_div">
            <ol class="popisky_div">
                <li class="popisek">
                    <h3 class="t1">T1</h3>
                    <p>Toto tlačítko funguje k přepínání výpisu. Možné výpisy: teplota, tlak, vlhkost, intenzita. </p>
                </li>
                <li class="popisek">
                    <h3 class="t1">T2</h3>
                    <p >Toto tlačítko nechává uspat zařízení.</p>
                </li>
                <li class="popisek">
                    <h3 id="rgb">RGB</h3>
                    <p>Tato RGB Led ukazuje stupnici hodnot. Modrá znamená nízká hodnota, zelená je průměrná/ideální hodnota a červená je vysoká hodnota daného výpisu.</p>
                </li>
                <li class="popisek">
                    <h3 id="lcd">LCD</h3>
                    <p>Na této obrazovce se zobrazuje výpis hodnot naměřené sensory Meteostanice. Jsou 4 možné hodnoty: teplota, tlak, vlhkost, intenzita.</p>
                </li>
                <li class="popisek">
                    <h3 id="fot">FOT</h3>
                    <p>Zde se zezhora nachází otvor na fotorezistor. Jeden ze sensorů Meteostanice. Měří intenzitu osvětlení. Nezakrývat!</p>
                </li>
            </ol>
             
                
        </div>
        
    
    </div>
    <p>Zde si prosím pročtěte důležité bezpečnostní a smluvní podmínky</p>
    <ol>
            <li>Meteostanice nesmí přijít do kontaktu s vodou! Je to elektronické zařízení a proto by se mohlo poškodit. Měření vlhkosti vzduchu tuto podmínku nemění.</li>
            <li>Nesahejte do obvodů Meteostanice, dokud není vypojena z napájení! Jsou 2 možné typy napájení - 9V baterií a modrým kabelem externě z krabičky Meteostanice</li>
            <li>Meteostanice není vytvořena k dlouhodobému použití ve venkovním prostředí. Zařízení by mohlo přestat fungovat z několika důvodů - déšť, blesk, přehřátí a další. </li>
            <li>Meteostanici držte raději dál od dětí. Nachází se v ní malé součástky, které dokáží být nebezpečné.</li>
            <li>Autoři projektu nenesou žádnou odpovědnost za škody na majetku či zdraví způsobené nesprávnou montáží, provozem nebo interpretací naměřených dat.</li>
            <li>Meteostanice není certifikovaný měřící přístroj. Veškerá data by měla být sice měřena velmi přesně, přesto Meteostanici nepoužívejte pro rozhodování ovlivňující zdraví nebo majetek.</li>
            <li>Jakákoli úprava čehokoli v rámci tohoto projektu (viz obsah projektu <a href="/dokumenty#obsah">zde</a>)je na vlastní riziko a nedoporučuje se.</li>
            <li>Pokud Meteostanice nefunguje, vinnen je poslední člověk jež s Meteostanicí manipuloval. Můžete se obrátit na jednoho z autorů, či vedocího práce, avšak NEZARUČUJE SE, že Meteostanice bude opravena.</li>
        </ol>






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

    .navod_template{
        /* border: 4px red solid; */
        display: flex;
        flex-direction: column;
        flex-wrap: wrap;
        gap: 4rem;
        margin: 5rem 0rem 5rem 0rem;

    }
    .navod_template img{
        height: 100%;
        width: 100%;
        transition: transform 0.5s ease;
        border-radius: 5%;
    }
    .navod_template img:hover{
        transform: scale(1.2);
    }
    .navod_template h2{
        text-align: center;
        font-size:  clamp(1.2rem, 1.8rem, 2.2rem);
    }
    .popisky_div{
        /* border: 2px green solid; */
        display: flex;
        flex-wrap: wrap;
        flex-direction: row;
        gap: 1rem;
        justify-content: center;
    }
    .popisky_div li{
        list-style: none;
    }
    .popisek{
        /* border: blue 2px dashed; */
        /* width: clamp(15%,25%,35%); */
        flex: 1 1 300px;
        max-width: 400px;
        padding: 2%;
        background-color:  #009fe3;
        display: flex;
        flex-direction: column;
        border-radius: 5%;
        transition: transform 0.3s ease;
    }
    .popisek:hover {
        
    transform: translateY(-5px); 
    transform: scale(1.05);
}
    .popisek h3{
        font-family: var(--font-mono);
        font-size: clamp(1rem, 1.5rem, 2rem);
        text-align: center;
        margin: 2%;
        padding: 1rem;
        
        
    }
    .t1{
        text-decoration: underline;
        text-decoration-color: yellow;
        
    }
    #rgb{
        text-decoration: underline;
        text-decoration-color: red;
    }
    #lcd{
        text-decoration: underline;
        text-decoration-color: aquamarine;
    }
    #fot{
        text-decoration: underline;
        text-decoration-color: blue;
    }
    .popisek p{
        font-size: clamp(0.5rem,1rem,1.5rem);
        background-color: rgb(228, 228, 228);
        padding: 5%;
        margin: 1em;
        flex-grow: 1;
        height: auto;
        border-radius: 2rem;
    }
    
</style>