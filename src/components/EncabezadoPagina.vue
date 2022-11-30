<template>
<head>
    <meta charset="utf-8">
	<title>Cabecera fija</title>

        <link rel="stylesheet" href="style.css">
</head>

<div class="encabezado">
    <ul class="encabezado__pagina">
        <div class="encabezado__pagina__menu">
            <button type="submit" class="menu"><img alt="menu" src="@/assets/botonmenu.png">
            </button>
        </div>
        <div class="encabezado__pagina__logo">
        <!-- <a href="#" class="encabezado__pagina__menu__logopagina"> 
                logo de la pagina
            </a>-->
            <img alt="logo" src="@/assets/logo.png">
        </div>
        <div class="encabezado__pagina__busqueda">
            <button type="submit" class="buscar"><img alt= "lupa" src="@/assets/lupita.png">
            </button>
            <input type="text" class="buscartermino" placeholder="Busqueda">
        </div>
        <div class="encabezado__pagina__versitio">
            <button type="submit" class="versitio"><img alt= "versitio" src="@/assets/versitio.png">
            </button>
            <a href="#" class="encabezado__pagina__versitio__texto"> 
                Ver sitio
            </a>
        </div>
        <div class="encabezado__pagina__campana">
            <button type="submit" class="campana"><img alt= "campana" src="@/assets/campanita.png">
            </button>
        </div>
        <div class="encabezado__pagina__usuario">
            <img alt="perfil" src="@/assets/perfil.png">
            <li class="encabezado__pagina__usuario__lista">
                <a href="#" class="encabezado__pagina__usuario__texto1"> 
                    Nombre Usuario
                </a>
                <a href="#" class="encabezado__pagina__usuario__texto2"> 
                    Rol Usuario
                </a>
            </li>
            <button type="submit" class="desplegable"><img alt= "desplegable" src="@/assets/desplegable.png">
            </button>
        </div>
    </ul>

</div>
</template>

<script>
export default {
    name: 'EncabezadoPagina'

}
</script>

<style lang="css" scoped>
    .encabezado {
        width: 100%;
        height: 10%;
        background-color:#fff;
        display: flex;
        justify-content: space-between;
        align-items: center;
        margin: 0;
        margin: 0;
    }
    .encabezado__pagina {
        display: flex;
        flex-direction: row;
        list-style: none;
        justify-content: space-around;
        align-items: center;
        display: flex;
        width: 100%;
        height:10%;
        border: solid 1px #CACDCE;
        border-radius: 5px;
        padding-right: 0px;
        margin: 0;
        font-style:initial;
        text-decoration: none;
    }
    .encabezado__pagina__menu {
        width: 5%;
        height: 5%;
        display:flex;
        /*background: transparent url('assets/logopagina.png') 0% 0% no-repeat padding-box;*/
    }

    .menu {
        width: 40px;
        height: 36px;
        border: 0%;
        background:#fff;
        text-align: center;
        border-color: transparent;
        color: #fff;
        font-size: 20px;
        cursor: pointer;
    }

    .menu img {
        height: 50%;
    }
    

    .encabezado__pagina__logo {
        width: 20%;
        height: 20%;
    }

    .encabezado__pagina__busqueda {
        width: 30%;
        height: 20%;
        display: flex;
        list-style: none;
        padding: 0%;
        margin: 0%;
    }
    .buscar {
        width: 40px;
        height: 36px;
        border: 1px solid #CACDCE;
        background:#fff;
        text-align: center;
        color: #fff;
        border-radius: 5px 0 0 5px;
        cursor: pointer;
        font-size: 20px;
    }
    .buscar img{
        height: 50%;
    }

    .buscartermino {
        display: flex;
        width: 100%;
        border: 1px;
        border-right: none;
        padding: 5px;
        height: 24px;
        border: solid 1px #CACDCE;
        border-radius: 0 5px 5px 0;
        outline: none;
        color: #9DBFAF;
    }

    .buscartermino:focus {
        color: #000;
    }

    .encabezado__pagina__versitio {

        height: 10%;
        width: 10%;
        display: flex;
        list-style: none;
        align-items: center;
        padding: 0%;
        margin: 0%;
    }
    
    .versitio {
        width: 40px;
        height: 36px;
        border: 0%;
        background:#fff;
        text-align: center;
        border-color: transparent;
        color: #fff;
        font-size: 20px;
        cursor: pointer;
    }
    .versitio img {
        height: 70%;
    }

    .encabezado__pagina__versitio__texto {
        align-items: center;
        font-style: open sans regular;
        text-decoration: none;
        color: #202124;
    }

    .encabezado__pagina__campana {
        height: 10%;
        width: 10%;
        display: flex;
        list-style: none;
        align-items: center;
        padding: 0%;
        margin: 0%;
    }

    .campana {
        width: 40px;
        height: 36px;
        border: 0%;
        background:#fff;
        text-align: center;
        border-color: transparent;
        color: #fff;
        font-size: 20px;
        cursor: pointer;
    }

    .campana img {
        height: 75%;
    }

    .encabezado__pagina__usuario {
        display: flex;
        list-style:circle;
        align-items: center;
        height: 50%;
    }

    .perfil img {
        height: 40%;
    }

    .encabezado__pagina__usuario__lista {
        display: flex;
        flex-direction: column;
    }

    .encabezado__pagina__usuario__texto1 {
        align-items:flex-start;
        font-style: open sans regular;
        text-decoration: none;
        color: #202124;
    }

    .encabezado__pagina__usuario__texto2 {
        align-items: center;
        font-style: open sans regular;
        text-decoration: none;
        color: #202124;
    }

    .desplegable {
        width: 40px;
        height: 36px;
        border: 0%;
        background:#fff;
        text-align: center;
        border-color: transparent;
        color: #fff;
        font-size: 20px;
        cursor: pointer;
    }

    .desplegable img {
        height: 30%;
    }

</style>