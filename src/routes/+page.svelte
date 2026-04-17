<div class="main">
    <div class="uvod"><div class="uvod_logo"><img src="logo_meteostanice.png" alt="logo meoteostanice" id="logo_meteostanice"></div><div class="uvod_pointer"><a href="#nav"><img src="pointer_2.svg" alt="pointer_2.svg" id="pointer"></a></div></div>
    <div class="mid"><nav class="navigace" id="nav"><div class="navigace_div"><a class="logo_nav" href="/"><img src="logo_meteostanice.png" alt="logo meteostanice navigace" id="logo_nav_id" ></a></div>
    <div class="navigace_div navigace_div_text"><a class="navigace_div_text_text " href="/">DOMŮ</a></div>
    <div class="navigace_div navigace_div_text"><a class="navigace_div_text_text " href="/navody">NÁVODY</a></div>
    <div class="navigace_div navigace_div_text"><a class="navigace_div_text_text" href="/dokumenty">VÝVOJ</a></div></nav>

    <div class="mid_text">    <h1 class="nadpis">Projekt meteostanice</h1>
    Představujeme Vám doprovodný web k školnímu projektu Meteostanice na předmět hardware. Mozkem celé meteostanice je mini počítač Arduino UNO R3, na něj jsou napojeny sensory, díky kterým jsme schopni s velkou přesností měřit 4 hodnoty: teplotu, tlak, vlhkost a instenzitu světla. Pro tento projekt jsme navrhli a vyrobili unikítní krabičku, udělanou přímo na použité komponenty.
    <div id="mid_1fotka"><div id="fotka_meteostanice_mid"><img src="logo_meteostanice.png" alt="fotka"></div><div>Takto vypadá finální vzhled meteostanice. Veškeré komponenty jsou uvnitř krabičky. Ta byla vytisknuta na 3D tiskárně ve škole. Materiál je _______ </div></div>
    <div id="mid_2fotka"><div>Takto vypadál návrh vzhledu meteostanice. Původně bylo plánováno ________.  </div><div id="fotka_meteostanice_mid_2"><img src="logo_meteostanice.png" alt="fotka"></div></div>
    <div id="Galerie"><div class="galerie_nadpis "><h2 class="nadpis">Galerie</h2></div><div class="galerie_foto"> 
        <img src="logo_meteostanice.png" alt="prvni" class="galerie_img" >
        <img src="logo_meteostanice.png" alt="druhy" class="galerie_img">
        <img src="logo_meteostanice.png" alt="treti" class="galerie_img">
        <img src="logo_meteostanice.png" alt="ctvrty" class="galerie_img">
        <img src="logo_meteostanice.png" alt="paty" class="galerie_img">
        <img src="logo_meteostanice.png" alt="sesty" class="galerie_img"></div></div>
    Další informace o tvorbě našeho projektu najdete <a href="/dokumenty">zde</a>. Před použitím si prosím pročtěte návod k použití naši meteostanice, který najdete <a href="/navody">zde</a>. Jsme rádi že jste navštívili náš web a pevně věříme že se Vám náš projekt líbí. 
</div>
</div>
    
</div>
<style>
 h1{
        text-align: center;
        margin-top: 2%;
        
    
    }
    .nadpis{
        font-family: var(--font-mono);
    }

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
    .mid{
        min-height: 100vh;
        font-size: 1.1rem;
        
    }
   
    .mid_text{
        padding: 5% 15% 5% 15%;
    }
#mid_1fotka {
    width: 100%;
    /* border: 1px green solid; */ /* Můžeš smazat, až to uvidíš hotové */
    padding: 5% 0;
    display: flex;
    flex-direction: row;
    gap: 4%;             /* Mezera mezi fotkou a textem */
    align-items: center; /* Vycentruje text vertikálně k fotce */
}

/* Levá polovina - kontejner pro fotku */
#fotka_meteostanice_mid {
    flex: 1;             /* Znamená: zaber 1 díl (přesně polovinu) */
    display: flex;
    justify-content: center;
}

#fotka_meteostanice_mid img {
    width: 100%;         /* Fotka vyplní celou svou levou polovinu */
    max-width: 400px;    /* Volitelné: aby nebyla na obřích monitorech moc velká */
    height: auto;
    border-radius: 8px;  /* Jen tip: vypadá to líp s mírným zaoblením */
}

/* Pravá polovina - kontejner pro text */
#mid_1fotka > div:last-child { 
    flex: 1;             /* Znamená: zaber taky 1 díl (druhou polovinu) */
    font-size: 1.1rem;   /* Trochu zvětšíme text, ať se to dobře čte */
    line-height: 1.6;    /* Větší řádkování pro čistší vzhled */
}

#Galerie{
    display: block;
    align-items: center;
    justify-content: center;
    border: 1px red dashed;
    
}
.galerie_nadpis{
    border: green 2px solid;
    text-align: center;
    margin-bottom: 5%;
}
.galerie_foto{
    display: flex;
    flex-wrap: wrap;
    border: 2px yellow solid;
    justify-content: center;
    gap: 5%;
    
}
.galerie_foto img{
    margin-bottom: 5%;
    width: 40%;
    height: auto;
    display: inline-block;
}

/* RESPONSIVITA: Na mobilu pod sebe */
@media (max-width: 768px) {
    #mid_1fotka {
        flex-direction: column; /* Na mobilu naskládat pod sebe */
        text-align: center;
    }
}
    #mid_2fotka{
         width: 100%;
    /* border: 1px green solid; */ /* Můžeš smazat, až to uvidíš hotové */
    padding: 5% 0;
    display: flex;
    flex-direction: row;
    gap: 4%;             /* Mezera mezi fotkou a textem */
    align-items: center; /* Vycentruje text vertikálně k fotce */
    margin: 0 0 5% 0;

    }
    #fotka_meteostanice_mid_2{
        flex: 1;             /* Znamená: zaber 1 díl (přesně polovinu) */
    display: flex;
    justify-content: center;
    }
    #fotka_meteostanice_mid_2 img {
    width: 100%;         /* Fotka vyplní celou svou levou polovinu */
    max-width: 400px;    /* Volitelné: aby nebyla na obřích monitorech moc velká */
    height: auto;
    border-radius: 8px;  /* Jen tip: vypadá to líp s mírným zaoblením */
}

/* Pravá polovina - kontejner pro text */
#mid_2fotka > div:first-child { 
    flex: 1;             /* Znamená: zaber taky 1 díl (druhou polovinu) */
    font-size: 1.1rem;   /* Trochu zvětšíme text, ať se to dobře čte */
    line-height: 1.6;    /* Větší řádkování pro čistší vzhled */
}

/* RESPONSIVITA: Na mobilu pod sebe */
@media (max-width: 768px) {
    #mid_2fotka {
        flex-direction: column-reverse; /* Na mobilu naskládat pod sebe */
        text-align: center;
    }
}






/* NOT MY WORK - UPDATED */
@media (max-width: 768px) {
    /* Oprava úvodní obrazovky */
    .uvod {
        justify-content: center; 
        gap: 5vh;
    }

    #logo_meteostanice {
        margin-top: 0;
        height: auto;
        width: 60vw; /* Trochu jsme zmenšili, aby zbyl prostor */
    }

    .uvod_logo {
        height: auto;
        width: auto;
    }

    .uvod_pointer {
        padding-top: 0;
        width: 12vw;
        height: auto;
    }

    
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
    .mid_text {
        padding: 5% 5%; 
    }
}

</style>