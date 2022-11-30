<template>

<head>
    <meta charset="utf-8">
	<title>Cabecera fija</title>

        <link rel="stylesheet" href="style.css">
</head>

<div class="contenidopagina">
    <ul class="contenidopagina__tarjeta">
        <div class="contenidopagina__tarjeta__infotienda">
            <button type="submit" class="enlace"><img alt="enlace" src="@/assets/logodelcampo.png">
            </button>
            <li class="contenidopagina__tarjeta__infotienda__lista">
                <h1>Del campo express</h1>
                <sub>URL de mi tienda en linea</sub>
                <a href="#" class="contenidopagina__tarjeta__infotienda__enlace"> 
                https://delcampoexpress.viveshops.co
                </a>
            </li>
        </div>
        <div class="contenidopagina__tarjeta__general">
            <div class="contenido__tarjeta__titulobarra">
                <h1 class="completa">Completa tu cuenta</h1>
                <div class="barracarga">
                    <span id="cargando"></span>
                <!--<div class="contenido__tarjeta__titulobarra__barra" style="height: 40px; width: 10px;">
                    <div class="progress-bar" role="progressbar" style="width: 25%;" aria-valuenow="0" aria-valuemin="0" aria-valuemax="100"></div>
                </div>-->
                </div>
                <div class="boton">
                    <button onclick="document.getElementById('modal')" data-toggle="modal" data-target="#emergente" class="botonregistro">registrar producto</button>
                </div>
            </div>
            <div class="contenidopagina__tarjeta__info">
                <div class="contenidopagina__tarjeta__instrucciones1">
                    <li class="parte1"><button type="submit" class="icono"><img alt="icono" src="@/assets/carpeta.png"></button> <a href="#" class="textoenlace"> Crear Producto</a></li>
                    <li class="parte1"><button type="submit" class="icono"><img alt="icono" src="@/assets/ubicacion.png"></button> <a href="#" class="textoenlace"> Definir Cobertura Envios</a></li>
                    <li class="parte1"><button type="submit" class="icono"><img alt="icono" src="@/assets/pestana.png"></button> <a href="#" class="textoenlace"> Agregar Metodo De Pago</a></li>
                    <li class="parte1"><button type="submit" class="icono"><img alt="icono" src="@/assets/mundo.png"></button> <a href="#" class="textoenlace"> Establecer Dominio</a></li>
                </div>
                <div class="contenidopagina__tarjeta__instrucciones2">   
                    <li class="parte1"><button type="submit" class="icono"><img alt="icono" src="@/assets/foto.png"></button> <a href="#" class="textoenlace"> Definir Logo Y Colores</a></li>
                    <li class="parte1"><button type="submit" class="icono"><img alt="icono" src="@/assets/regalo.png"></button> <a href="#" class="textoenlace"> Personalizar plantilla</a></li>
                    <li class="parte1"><button type="submit" class="icono"><img alt="icono" src="@/assets/megafono.png"></button> <a href="#" class="textoenlace"> Activar Campañas</a></li>
                    <li class="parte1"><button type="submit" class="icono"><img alt="icono" src="@/assets/id.png"></button> <a href="#" class="textoenlace"> Completar Documentos</a></li>
                </div>
            </div>
        </div>
    </ul>
</div>
</template>

<script>

/*var i = 0;
function move() {
  if (i == 0) {
    i = 1;
    var elem = document.getElementById("barra");
    var width = 10;
    var id = setInterval(frame, 10);
    function frame() {
      if (width >= 100) {
        clearInterval(id);
        i = 0;
      } else {
        width++;
        elem.style.width = width + "%";
        elem.innerHTML = width  + "%";
      }
    }
  }
}*/

export default {
    name: 'ContenidoPagina'

}
</script>

<style lang="css" scoped>
    .contenidopagina {
        width: 100%;
        height: 80%;
        background-color: #F5F5F5;
        display: flex;
        justify-content: center;
        align-items: center;
        box-shadow: 4px;
    }

    .contenidopagina__tarjeta {
        display: flex;
        flex-direction: row;
        list-style: none;
        justify-content:space-around;
        align-items: center;
        padding-left: 0%;
        padding-right: 5%;
        width: 90%;
        height: 300px;
        box-shadow: 0px 5px 5px #00000012;
        border: 1px solid #EBEDED;
        border-radius: 6px;
        color: #000;
        background-color: #fff;
    }

    .completa {
        font-size: 120%;
    }

    .contenidopagina__tarjeta__infotienda {
        width: 30%;
        height: 90%;
        display:flex;
        align-items: center;
    }

    .enlace {
        width: 30%;
        height: 40%;
        border: 0%;
        background:#fff;
        text-align: center;
        color: #fff;
        font-size: 20px;
        cursor: pointer;
        box-shadow: 0px 3px 6px #00000012;
        border: 1px solid #EBEDED;
        border-radius: 7px;
    }

    .enlace img {
        width: 100%;
        height: 30%;
    }

    .contenidopagina__tarjeta__general {
        display: block;
        width: 40%;
        justify-content: space-between;
    }

    .contenidopagina__tarjeta__info {
        display: flex;
        text-align: left;
        justify-content: space-between;
    }

    .contenido__tarjeta__titulobarra {
        display: flex;
        align-items: center;
        justify-content: space-between;
    }

    .barracarga {
        height: 2%;
        position: absolute;
        width: 20%;
        background: #E0E0E0;
        border-radius: 10px;
        margin-top: 0%;
        margin-left:15%;
  
    }
    
    #cargando {
        display: flex;
        height: 60%;
        width: 10px;
        border-radius: 8px;
        margin: 3px;
        background: #005CAB;
        transition: 1s ease 0.3s;
    }

    .progress-bar {
        display: flex;
    }

    .contenidopagina__tarjeta__instrucciones1 {
        align-items:left;
        align-content:left;
        margin: left ;
    }

    .contenidopagina__tarjeta__instrucciones2 {
        align-items:left;
        align-content:left;
        margin: left ;
        padding-left: 1%;
    }

    .parte1 {
        align-items:left;
        align-content:left;
        margin: left ;
    }


    .icono {
        width: 40px;
        height: 36px;
        border: 0%;
        background:#fff;
        text-align: left;
        border-color: transparent;
        color: #fff;
        font-size: 20px;
        cursor: pointer;
    }

    .icono img {
        width: 70% ;
        height: 50% ;
    }

    .textoenlace {
        align-items: left;
        font-style: open sans regular;
        text-decoration: none;
        color: #202124;
    }

    .textoenlace :active {
        align-items: center;
        font-style: open sans regular;
        text-decoration: none;
        color: #202124;
        opacity: 60%;
    }

    #myProgress {
        width: 100%;
        background-color: #ddd;
    }

    #myBar {
        width: 10%;
        height: 30px;
        background-color: #04AA6D;
        text-align: center;
        line-height: 30px;
        color: white;
    }

</style>