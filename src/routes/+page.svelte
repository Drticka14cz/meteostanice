<div class="main">
    <div class="uvod"><div class="uvod_logo"><img src="logo_meteostanice.png" alt="logo meoteostanice" id="logo_meteostanice"></div></div>
    <div class="mid">Pica</div>
</div>
<style>
    .uvod{
        background-image:url("meteo_pozadi.png");
        background-size: cover;
        background-repeat: repeat;
        background-position: center;
        height: 100vh;
        width: 100vw;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        animation: mraky_repeat infinite timing-function delay iteration-count direction fill-mode;
    }
    .uvod_logo{
        height: 40vh;
        width: 40vw;
        border: red dashed 2px;

    }
    #logo_meteostanice{
        height: 40vh;
      
    }
    .mid{
        min-height: 100vh;
    }

</style>