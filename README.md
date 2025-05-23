<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mundo  Cuento</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f0f8ff;
            margin: 0;
            padding: 0;
            text-align: center;
        }

        header {
            background-color: #4CAF50;
            color: white;
            padding: 20px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            flex-wrap: wrap;
        }

        header h1 {
            margin: 0;
        }

        .busqueda {
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .busqueda input {
            padding: 10px;
            width: 250px;
            font-size: 16px;
            border: 2px solid #4CAF50;
            border-radius: 4px;
        }

        .busqueda button {
            padding: 10px 15px;
            background-color: #4CAF50;
            color: white;
            border: none;
            border-radius: 4px;
            cursor: pointer;
        }

        .busqueda button:hover {
            background-color: #45a049;
        }

        .cuento-imagen {
            width: 300px;
            height: 400px;
            margin: 20px;
            cursor: pointer;
            border-radius: 8px;
            transition: transform 0.3s;
        }

        .cuento-imagen:hover {
            transform: scale(1.05);
        }

        .contenido-cuento {
            display: none;
            background-color: #ffffff;
            padding: 20px;
            margin: 20px auto;
            max-width: 800px;
            border-radius: 8px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            text-align: left;
            line-height: 1.6;
        }

        .cuento-img {
            max-width: 100%;
            border-radius: 8px;
            margin-top: 20px;
        }

        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 10px;
            position: fixed;
            width: 100%;
            bottom: 0;
        }
    </style>
</head>
<body>

<header>
    <h1> Mundo Cuento</h1>
    <!-- Sección de búsqueda al lado del título -->
    <div class="busqueda">
        <input type="text" id="busqueda-input" placeholder="Buscar cuento..." oninput="buscarCuento()">
        <button onclick="buscarCuento()">Buscar</button>
    </div>
</header>

<div>
    <img class="cuento-imagen" src="https://losresumenes.com/wp-content/uploads/2023/11/Hermanos-Grimm-Caperucita-Roja-Imagen-1.jpg" alt="Caperucita Roja" onclick="mostrarCuento('caperucita-roja')" data-cuento="Caperucita Roja">
    <img class="cuento-imagen" src="https://i1.sndcdn.com/artworks-000412660605-3xgsjx-t1080x1080.jpg" alt="Los Tres Chanchitos" onclick="mostrarCuento('tres-chanchitos')" data-cuento="Los Tres Chanchitos">
    <img class="cuento-imagen" src="https://images.cdn1.buscalibre.com/fit-in/360x360/b7/ed/b7edbff90292aaf25e23ae6fd96c2053.jpg" alt="El Hada de los Dientes" onclick="mostrarCuento('hada-dientes')" data-cuento="El Hada de los Dientes">
</div>

<!-- Cuento de Caperucita Roja -->
<div id="caperucita-roja" class="contenido-cuento">
    <h2>Caperucita Roja</h2>
    <img class="cuento-img" src="https://losresumenes.com/wp-content/uploads/2023/11/Hermanos-Grimm-Caperucita-Roja-Imagen-1.jpg" alt" alt="Caperucita Roja">
    <p>Había una vez una niña llamada Caperucita Roja, que vivía en una pequeña aldea. Un día, su madre le pidió que llevara una cesta con comida a su abuela, que vivía en el bosque. Caperucita Roja, mientras caminaba por el bosque, se encontró con el lobo, que la engañó y la hizo contarle a dónde iba.</p>
    <p>El lobo, al saber la dirección, llegó antes que ella a la casa de la abuela. Allí, devoró a la anciana y se disfrazó de ella, esperando que Caperucita Roja llegara. Cuando la niña llegó a la casa, se sorprendió al ver a "su abuela" en la cama, pero notó algo extraño en ella.</p>
    <p>"Abuela, qué grandes ojos tienes", dijo Caperucita. "Son para verte mejor, querida", respondió el lobo disfrazado. "Abuela, qué grandes orejas tienes", dijo la niña. "Son para oírte mejor, querida", contestó el lobo. "Abuela, qué grandes dientes tienes", dijo Caperucita Roja. "Son para comerte mejor", rugió el lobo, saltando de la cama para devorarla.</p>
    <p>En ese momento, un cazador que pasaba por allí escuchó el ruido y entró en la casa. Con un solo golpe, mató al lobo, rescató a la abuela y salvó a Caperucita Roja. Desde entonces, Caperucita Roja aprendió a no hablar con extraños ni a desviarse del camino.</p>
</div>

<!-- Cuento de Los Tres Chanchitos -->
<div id="tres-chanchitos" class="contenido-cuento">
    <h2>Los Tres Chanchitos</h2>
    <img class="cuento-img" src="https://i1.sndcdn.com/artworks-000412660605-3xgsjx-t1080x1080.jpg" alt="Los Tres Chanchitos">
    <p>Había una vez tres cerditos que vivían en el bosque. Un día, decidieron construir sus casas para protegerse del feroz lobo que rondaba por allí. El primer cerdito, que era muy perezoso, construyó su casa de paja. El segundo cerdito, que era un poco más trabajador, construyó su casa de madera. El tercer cerdito, que era muy sabio, decidió construir su casa de ladrillos.</p>
    <p>El lobo llegó a la casa de paja y sopló tan fuerte que derribó la casa y se comió al primer cerdito. Luego, fue a la casa de madera y sopló tan fuerte como pudo, hasta que también derribó la casa y devoró al segundo cerdito.</p>
    <p>Finalmente, el lobo llegó a la casa de ladrillos. Sopló con todas sus fuerzas, pero la casa no se movió ni un poco. El lobo, enfadado, trató de entrar por la chimenea, pero el cerdito más sabio había preparado una trampa. El lobo cayó en una olla de agua hirviendo y salió corriendo, nunca más volvió a molestar a los cerditos.</p>
    <p>Desde ese día, los tres cerditos vivieron felices y seguros en su casa de ladrillos, y aprendieron la importancia de la perseverancia y el trabajo duro.</p>
</div>

<!-- Cuento de El Hada de los Dientes -->
<div id="hada-dientes" class="contenido-cuento">
    <h2>El Hada de los Dientes</h2>
    <img class="cuento-img" src="https://images.cdn1.buscalibre.com/fit-in/360x360/b7/ed/b7edbff90292aaf25e23ae6fd96c2053.jpg" alt="El Hada de los Dientes">
    <p>Había una vez una niña llamada Sofía que perdió su primer diente de leche. Sofía, emocionada, puso su diente debajo de la almohada antes de irse a dormir, esperando la visita de un ser mágico.</p>
    <p>Durante la noche, el Hada de los Dientes llegó volando con su varita brillante y recogió el diente de Sofía, dejando a cambio una moneda como recompensa. Pero, antes de irse, el Hada le susurró al oído: "Recuerda siempre cuidar tus dientes, porque cada uno es un pequeño tesoro que tu cuerpo te da".</p>
    <p>Al día siguiente, Sofía se despertó y encontró la moneda bajo su almohada, asombrada y feliz por la magia que había vivido. Desde entonces, cada vez que perdía un diente, sabía que el Hada de los Dientes siempre estaría allí para visitar y dejarle un pequeño obsequio, como un recordatorio de lo importante que es cuidar nuestra salud dental.</p>
</div>

<footer>
    <p>&copy; 2024  Mundo  Cuento - JHOEL AGUILAR </p>
</footer>

<script>
    function mostrarCuento(id) {
        // Ocultar todos los cuentos
        var cuentos = document.querySelectorAll('.contenido-cuento');
        for (var i = 0; i < cuentos.length; i++) {
            cuentos[i].style.display = 'none';
        }

        // Mostrar el cuento seleccionado
        var cuentoSeleccionado = document.getElementById(id);
        if (cuentoSeleccionado) {
            cuentoSeleccionado.style.display = 'block';
        }
    }

    function buscarCuento() {
        var input = document.getElementById('busqueda-input').value.toLowerCase();
        var cuentos = document.querySelectorAll('.cuento-imagen');

        for (var i = 0; i < cuentos.length; i++) {
            var cuentoTitulo = cuentos[i].getAttribute('data-cuento').toLowerCase();
            if (cuentoTitulo.includes(input)) {
                cuentos[i].style.display = 'block';
            } else {
                cuentos[i].style.display = 'none';
            }
        }
    }
</script>

</body>
</html>
