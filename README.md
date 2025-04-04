<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Pedidos</title>
    <link rel="stylesheet" href="style.css">
    
</head>
<body>
 
    <section class="contenido">
        <div class="imagen-comida">
            <img src="IMG/Img-1.png">
            <!-- Botón para mostrar el formulario -->
            <button class="boton-ordenar" onclick="mostrarFormulario()">Ordenar Gelatina</button>
        </div>
        
        <!-- Formulario que aparece al hacer clic en "ordenar gelatinas" -->
        <div id="formulario-orden" class="formulario oculto">
            <h2>Selecciona tu pedido</h2>
            <form action="procesar-pedido.html" method="post">
                <label for="sabores">Sabores:</label>
                <select id="sabores" name="sabores" required>
                    <option value="gelatinas">Gelatinas de fresa con frutas</option>
                    <option value="gelatinas">Gelatinas de uva con frutas</option>
                    <option value="gelatinas">Gelatinas de piña con fruta</option>
                    <option value="gelatinas">Gelatinas de fresa con leche</option>
                    <option value="gelatinas">Gelatinas frambruesa con leche</option>
                    <option value="gelatinas">Gelatinas de piña con leche</option>
                    <option value="gelatinas">Gelatinas de fresa con leche y chocolate </option>
                    <option value="gelatinas">Gelatinas normales de fresa  </option>
                    <option value="gelatinas">Gelatinas normales uvas</option>
                    <option value="gelatinas">Gelatinas normales frambruesa </option>
                    <option value="gelatinas">Gelatinas normales piña</option>
                <br>
                
                

                <label for="cantidad">Cantidad:</label>
                <input type="number" id="cantidad" name="cantidad" min="1" max="20" value="1" required>
                <br>

                <button type="submit" class="boton-enviar">Enviar Pedido</button>
            </form>
        </div>
    </section>


<script src="pedi.js"></script>
</body>
</html># GELATIXIOSA


* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

/* Estilo general de la página */
body {
    font-family: Arial, sans-serif;
    color: #333;
    text-align: (24, 4, 4) center;
}

/* Estilo para el encabezado */



/* Estilo para las secciones con imágenes */
.contenido {
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 50px;
    margin-top: 30px;
    flex-direction: column;
}

.imagen-comida {
    text-align: center;
}

.imagen-comida img {
    width: 300px;
    height: auto;
    border-radius: 8px;
   
}

.imagen-comida p {
    margin-top: 10px;
    font-size: 1.1em;
    color: #fe0000;
}

/* Estilo del botón de ordenar */
.boton-ordenar {

    padding: 15px 30px;
    font-size: 1.2em;
    border: none;
    border-radius: 8px;
    cursor: pointer;
    text-decoration: none;
    margin-top: 20px;
    transition: background-color 0.3s ease;
}


/* Estilo para el formulario de pedido */
.formulario {
    margin-top: 20px;
    padding: 20px;
    border-radius: 8px;

}

.formulario label {
    font-size: 1.1em;
    margin-bottom: 10px;
    display: block;
}

.formulario select,
.formulario input {
    padding: 10px;
    font-size: 1em;
    margin-top: 10px;
    margin-bottom: 20px;
    border-radius: 5px;
    border: 1px ;
    width: 100%;
    max-width: 300px;
}

.boton-enviar {
    padding: 15px 30px;
    font-size: 1.2em;
    border: none;
    border-radius: 8px;
    cursor: pointer;
    transition: background-color 0.3s ease;
}

.boton-enviar:hover {
    background-color: #ff0000; /* Rojo más oscuro */
}

/* Estilo para ocultar el formulario */
.oculto {
    display: none;
}

footer {
    margin-top: 40px;
    padding: 10px 0;
}

