<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Página web con políticas y contacto.">
    <title>Trabalhos em Foz do Iguaçu</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <nav>
            <ul>
                <li><a href="#inicio">Inicio</a></li>
                <li><a href="Política de privacidad.html">Politica de privacidad</a></li>
                <li><a href="Política de cookies.html">Política de cookies</a></li>
                <li><a href="Aviso legal.html">Aviso legal</a></li>
                <li><a href="Contacto.html">Contacto</a></li>
                <li><a href="Quiénes somos.html">Quiénes somos</a></li>
                <li><a href="Términos de uso.html">Términos de uso</a></li>
<form id="barra-busqueda">
    <input type="text" id="busqueda" placeholder="Buscar..." onkeyup="buscarContenido()">
</form>

<script>
function buscarContenido() {
    let query = document.getElementById("busqueda").value.toLowerCase();
    let contenido = document.getElementById("contenido").getElementsByTagName("p");

    for (let i = 0; i < contenido.length; i++) {
        let text = contenido[i].textContent || contenido[i].innerText;
        if (text.toLowerCase().indexOf(query) > -1) {
            contenido[i].style.display = "";
        } else {
            contenido[i].style.display = "none";
        }
    }
}
</script>
                
            </ul>
        </nav>
    </header>

    </main>

    <aside>
        <h3>Categorías</h3>
        <ul>
            <li><a href="Restaurantes.html">Restaurantes</a></li>
            <li><a href="Hotel.html">Hotel</a></li>
            <li><a href="Prefeitura.html">Prefeitura</a></li>
            <li><a href="Mercado.html">Mercado</a></li>
        </ul>
    </aside>

    <section id="paginacion">
        <nav>
            <ul>
                <li><a href="#">« Anterior</a></li>
                <li><a href="#">1</a></li>
                <li><a href="#">2</a></li>
                <li><a href="#">3</a></li>
                <li><a href="#">Siguiente »</a></li>
            </ul>
        </nav>
    </section>

    <footer>
        
        <p>&copy; Todos los derechos reservados.</p>
    </footer>

    <script src="script.js"></script>
</body>
</html>
