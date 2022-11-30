<template>

<head>
    <meta charset="utf-8">
	<title>Cabecera fija</title>

        <link rel="stylesheet" href="style.css">
</head>

<div class="registro">
    <ul class="registro__pestana">
        <h1>Registro de Producto</h1>
        <div class="registro__pestana__infoproducto">
            <b class="titulo">Información del Producto</b>
            <div class="registro__pestana__infoproducto__categoria">
                <a class="subtitulo">Categoria</a>
                <select name="categoria" id="categoria" placeholder="Selecciona...">
                    <option value="Selecciona...">Selecciona...</option>
                    <option value="Categoria 1">Categoria 1</option>
                    <option value="Categoria 2">Categoria 2</option>
                    <option value="Categoria 3">Categoria 3</option>
                    <option value="Categoria 4">Categoria 4</option>
                </select>
            </div>
            <div class="registro__pestana__infoproducto__texto">
                <a class="subtitulo">Titulo</a>
                <input type="text" class="datoproducto" placeholder="Titulo del Producto">
            </div>
            <div class="registro__pestana__infoproducto__texto">
                <a class="subtitulo">Descripción</a>
                <input type="text" class="datoproducto" placeholder="Descripción del Producto">
            </div>
            <div class="registro__pestana__infoproducto__texto">
                <a class="subtitulo">Descripción Pro</a>
                <input type="text" class="datoproducto1" placeholder="Descripción detallada del Producto">
            </div>  
        </div>
        <div class="registro__pestana__variantes">
            <b class="titulo">Variantes</b>
            <div class="registro__pestana__variantes__eleccion">
                <select name="Talla" id="categoria2" placeholder="Talla">
                    <option value="Talla">Talla</option>
                    <option value="Talla XXS">Talla XXS</option>
                    <option value="Talla XS">Talla XS</option>
                    <option value="Talla S">Talla S</option>
                    <option value="Talla M">Talla M</option>
                    <option value="Talla L">Talla L</option>
                    <option value="Talla XL">Talla XL</option>
                </select>
                <select name="Color" id="categoria2" placeholder="Color">
                    <option value="Color">Color</option>
                    <option value="Azul">Azul</option>
                    <option value="Amarillo">Amarillo</option>
                    <option value="Rojo">Rojo</option>
                    <option value="Verde">Verde</option>
                    <option value="Blanco">Blanco</option>
                    <option value="Negro">Negro</option>
                </select>
                <select name="Sabor" id="categoria2" placeholder="Sabor">
                    <option value="Sabor">Sabor</option>
                    <option value="Chocolate">Chocolate</option>
                    <option value="Fresa">Fresa</option>
                    <option value="Vainilla">Vainilla</option>
                </select>
            </div>
            <li class="maslista"><button type="submit" class="mas"><img alt="mas" src="@/assets/mas.png"></button> <a href="#" class="mastexto"> Agregar grupos de toppings</a></li>
        </div>
        <div class="registro__pestana__preciodisponibilidad">
            <b class="titulo">Precio y Disponibilidad</b>
            <div class="registro__pestana__preciodisponibilidad__espacios">
                <div class="registro__pestana__preciodisponibilidad__parte1">
                    <div class="registro__pestana__preciodisponibilidad__parte1__titulotexto">
                        <a class="subtitulo2">Cantidad</a>
                        <input type="text" class="datopredis">
                    </div>
                    <div class="registro__pestana__preciodisponibilidad__parte1__titulotexto">
                        <a class="subtitulo2">SKU</a>
                        <input type="text" class="datopredis">
                    </div>
                </div>
                <div class="registro__pestana__preciodisponibilidad__parte1">
                    <div class="registro__pestana__preciodisponibilidad__parte1__titulotexto">
                        <a class="subtitulo2">Moneda</a>
                        <input type="text" class="datopredis">
                    </div>
                    <div class="registro__pestana__preciodisponibilidad__parte1__titulotexto">
                        <a class="subtitulo2">Precio</a>
                        <input type="text" class="datopredis">
                    </div>
                </div>
            </div>
        </div>
        <div class="registro__pestana__dimensiones">
            <b class="titulo">Dimensiones</b>
            <div class="registro__pestana__dimensiones1">
                <div class="registro__pestana__dimensiones__datos">
                    <div class="registro__pestana__dimensiones__datos__dato">
                        <a class="subtitulo3">Peso</a>
                        <div class="dimensiondato">
                            <input type="text" class="dimensiones">
                            <a class="medida">Grs</a>
                        </div>
                    </div>
                    <div class="registro__pestana__dimensiones__datos__dato">
                        <a class="subtitulo3">Alto</a>
                        <div class="dimensiondato">
                            <input type="text" class="dimensiones">
                            <a class="medida">Cm</a>
                        </div>
                    </div>
                    <div class="registro__pestana__dimensiones__datos__dato">
                        <a class="subtitulo3">Ancho</a>
                        <div class="dimensiondato">
                            <input type="text" class="dimensiones">
                            <a class="medida">Cm</a>
                        </div>
                    </div>
                    <div class="registro__pestana__dimensiones__datos__dato">
                        <a class="subtitulo3">Profundo</a>
                        <div class="dimensiondato">
                            <input type="text" class="dimensiones">
                            <a class="medida">Cm</a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class="registro__pestana__fotosdelproducto">


        </div>
        <div class="registro__pestana__botones">
            <div class="registro__pestana__botones__opcion">
                <button type="submit" class="opcion"><a class="textoopcion">Cancelar</a>
                </button>
                <button type="submit" class="opcion"><a class="textoopcion">Guardar</a>
                </button>
            </div>
        </div>
    </ul>
</div>
</template>

<script>
export default {
    name: 'RegistroProducto',
}
</script>

<style>
.registro {
    width: 50%;
    height: 50%;
    background-color: #F5F5F5;
    display: flex;
    justify-content: center;
    margin: auto;
    box-shadow: 4px;
    font-family:'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
}

.registro__pestana {
    display: flex;
    flex-direction: column;
    list-style: none;
    padding-left: 0%;
    padding-right: 5%;
    width: 90%;
    height: auto;
    margin-bottom: 200px;
    box-shadow: 0px 8px 8px #00000012;
    border: 1px solid #EBEDED;
    border-radius: 6px;
    color: #000;
    background-color: #fff;
}

registro__pestana__infoproducto {
    display: flex;
    flex-direction: column;
    justify-content:space-around;
    align-items: left;
    align-content: left;
    text-align: left;
}

.titulo {
    margin: 5px;
    text-align: left;
    
}

.subtitulo {
    margin: 5px;
    text-align: left;
    margin-left: 20%;
}

#categoria {
    width: 61%;
    height: 35px;
    background:#F5F5F5;
    margin-left: 20%;
    border: solid 2px #DDDFDF;
    border-radius: 5px;
    margin-bottom: 15px;
    text-decoration-color: #909798;
}

.registro__pestana__infoproducto__categoria {
    display: flex;
    flex-direction: column;
}

.registro__pestana__infoproducto__texto {
    display: flex;
    flex-direction: column;
}

.datoproducto {
    width: 60%;
    height: 30px;
    background:#F5F5F5;
    margin-left: 20%;
    border: solid 2px #DDDFDF;
    border-radius: 5px;
    margin-bottom: 15px;

}

.datoproducto1 {
    width: 60%;
    height: 70px;
    background:#F5F5F5;
    margin-left: 20%;
    border: solid 2px #DDDFDF;
    border-radius: 5px;
    margin-bottom: 15px;
    text-align:top;
}

.registro__pestana__variantes__eleccion {
    display: flex;
    flex-direction: column;
}

#categoria2 {
    width: 61%;
    height: 50px;
    background: #F5F5F5;
    margin-left: 20%;
    margin-top: 15px;
    border-color: transparent;
    border-radius: 10px;
    text-decoration-color: #909798;
    font-size: large;
    box-shadow: 0px 3px 3px #00000012;
}

.maslista {
    display: flex;
    align-items:center;
    align-content:center;
    margin-left: 20% ;
    margin-top: 20px;
}

.mas {
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

.mas img {
    width: 70% ;
    height: 50% ;
}

.mastexto {
    text-decoration: none;
    color: #005CAB;
}

.registro__pestana__preciodisponibilidad__espacios {
    display: flex;
    flex-direction: column;
    justify-content:space-between;
    align-items: left;
    align-content: left;
    text-align: left;
    margin-top: 20px;
}

.registro__pestana__preciodisponibilidad__parte1 {
    display: flex;
    flex-direction: row;
    justify-content:center;
}

.registro__pestana__preciodisponibilidad__parte1__titulotexto {
    display: flex;
    flex-direction: column;
    justify-content:center;
}

.datopredis {
    width: 90%;
    height: 30px;
    background:#F5F5F5;
    border: solid 2px #DDDFDF;
    border-radius: 5px;
    margin-bottom: 15px;
}

.registro__pestana__dimensiones {
    display: flex;
    flex-direction: column;
    align-items: center;
}

.registro__pestana__dimensiones1 {
    display: flex;
    margin-left: 20%;
}

.registro__pestana__dimensiones__datos {
    display: flex;
    flex-direction: row;
    justify-content:baseline;
    align-items: center;
}

.registro__pestana__dimensiones__datos__dato {
    display: flex;
    flex-direction: column;
    align-items:baseline;
    text-align: center;
}

.dimensiones {
    width: 40%;
    height: 30px;
    background:#F5F5F5;
    border: solid 2px #DDDFDF;
    border-radius: 5px;
    margin-bottom: 30px;
}

.dimensiondato {
    display: flex;
    flex-direction: row;
    align-items: left;
}

.registro__pestana__botones {
    display: center;
    flex-direction: row;
    align-items: center;
    justify-content: space-between;
    margin-left: 20%;
    margin-right: 20%;
}

.registro__pestana__botones__opcion {
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: space-between;
}

.textoopcion {
    color: #fff;
    font-size: large;
}

.opcion {
    background: #005CAB;
    border-color: transparent;
    border-radius:5px;
    height: 50px;
    width: 60%;
    cursor: pointer;
    margin-bottom: 40px;
    
}

</style>