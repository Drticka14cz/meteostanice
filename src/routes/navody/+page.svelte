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
</style>