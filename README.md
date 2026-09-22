<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Zapatillas M | Nueva Colección</title>

  <style>
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
      font-family: Arial, sans-serif;
    }

    body {
      background: #f7f7f7;
      color: #111;
    }

    /* HEADER */
    header {
      background: #fff;
      padding: 18px 6%;
      display: flex;
      align-items: center;
      justify-content: space-between;
      border-bottom: 1px solid #ddd;
      position: sticky;
      top: 0;
      z-index: 100;
    }

    .logo {
      font-size: 32px;
      font-weight: bold;
      letter-spacing: 4px;
    }

    nav a {
      color: #111;
      text-decoration: none;
      margin-left: 25px;
      font-size: 15px;
      font-weight: bold;
    }

    nav a:hover {
      text-decoration: underline;
    }

    /* INICIO */
    .hero {
      min-height: 480px;
      display: flex;
      align-items: center;
      justify-content: center;
      text-align: center;
      background: #111;
      color: white;
      padding: 40px 20px;
    }

    .hero h1 {
      font-size: 55px;
      margin-bottom: 15px;
    }

    .hero p {
      font-size: 20px;
      margin-bottom: 30px;
    }

    .btn {
      display: inline-block;
      padding: 14px 30px;
      background: white;
      color: #111;
      text-decoration: none;
      border-radius: 5px;
      font-weight: bold;
      border: none;
      cursor: pointer;
    }

    .btn:hover {
      opacity: .8;
    }

    /* SECCIONES */
    section {
      padding: 60px 6%;
    }

    .titulo {
      text-align: center;
      margin-bottom: 35px;
    }

    .titulo h2 {
      font-size: 32px;
      margin-bottom: 10px;
    }

    .titulo p {
      color: #666;
    }

    /* FILTROS */
    .filtros {
      display: flex;
      justify-content: center;
      gap: 12px;
      flex-wrap: wrap;
      margin-bottom: 35px;
    }

    .filtros input,
    .filtros select {
      padding: 12px;
      border: 1px solid #ccc;
      border-radius: 5px;
      background: white;
    }

    /* PRODUCTOS */
    .productos {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(230px, 1fr));
      gap: 25px;
    }

    .producto {
      background: white;
      border-radius: 10px;
      overflow: hidden;
      box-shadow: 0 3px 12px rgba(0,0,0,.08);
      transition: .2s;
    }

    .producto:hover {
      transform: translateY(-5px);
    }

    .producto img {
      width: 100%;
      height: 270px;
      object-fit: cover;
      background: #eee;
    }

    .producto-info {
      padding: 18px;
    }

    .producto-info h3 {
      margin-bottom: 8px;
    }

    .precio {
      font-size: 20px;
      font-weight: bold;
      margin-bottom: 12px;
    }

    .tallas {
      color: #666;
      font-size: 14px;
      margin-bottom: 15px;
    }

    .comprar {
      width: 100%;
      background: #111;
      color: white;
      border: none;
      padding: 13px;
      border-radius: 5px;
      cursor: pointer;
      font-weight: bold;
    }

    .comprar:hover {
      background: #333;
    }

    /* CLIENTES */
    .clientes {
      background: white;
    }

    .comentarios {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
      gap: 20px;
    }

    .comentario {
      background: #f5f5f5;
      padding: 25px;
      border-radius: 10px;
    }

    .estrellas {
      margin-bottom: 10px;
    }

    /* ADMIN */
    .admin {
      background: #111;
      color: white;
    }

    .admin-box {
      max-width: 700px;
      margin: auto;
      background: white;
      color: #111;
      padding: 30px;
      border-radius: 10px;
    }

    .admin-box input,
    .admin-box textarea,
    .admin-box select {
      width: 100%;
      padding: 12px;
      margin: 8px 0 15px;
      border: 1px solid #ccc;
      border-radius: 5px;
    }

    .admin-box button {
      width: 100%;
      padding: 14px;
      border: none;
      background: #111;
      color: white;
      cursor: pointer;
      border-radius: 5px;
      font-weight: bold;
    }

    /* FOOTER */
    footer {
      background: #000;
      color: white;
      text-align: center;
      padding: 30px;
    }

    /* WHATSAPP */
    .whatsapp {
      position: fixed;
      right: 20px;
      bottom: 20px;
      background: #25d366;
      color: white;
      width: 60px;
      height: 60px;
      border-radius: 50%;
      display: flex;
      align-items: center;
      justify-content: center;
      text-decoration: none;
      font-size: 28px;
      box-shadow: 0 4px 15px rgba(0,0,0,.25);
      z-index: 200;
    }

    @media(max-width:700px) {
      header {
        flex-direction: column;
        gap: 12px;
      }

      nav a {
        margin: 0 7px;
      }

      .hero h1 {
        font-size: 40px;
      }
    }
  </style>
</head>

<body>

<header>
  <div class="logo">M</div>

  <nav>
    <a href="#inicio">INICIO</a>
    <a href="#catalogo">CATÁLOGO</a>
    <a href="#clientes">CLIENTES</a>
    <a href="#admin">ADMIN</a>
  </nav>
</header>


<!-- INICIO -->
<section class="hero" id="inicio">
  <div>
    <h1>NUEVA COLECCIÓN</h1>
    <p>Zapatillas que combinan estilo y comodidad.</p>
    <a href="#catalogo" class="btn">COMPRAR</a>
  </div>
</section>


<!-- CATÁLOGO -->
<section id="catalogo">

  <div class="titulo">
    <h2>NUESTRAS ZAPATILLAS</h2>
    <p>Encuentra tu próximo par favorito.</p>
  </div>

  <!-- FILTROS -->
  <div class="filtros">

    <input
      type="text"
      id="busqueda"
      placeholder="Buscar zapatillas..."
      onkeyup="filtrarProductos()"
    >

    <select id="tallaFiltro" onchange="filtrarProductos()">
      <option value="">Todas las tallas</option>
      <option value="35">35</option>
      <option value="36">36</option>
      <option value="37">37</option>
      <option value="38">38</option>
      <option value="39">39</option>
      <option value="40">40</option>
    </select>

    <select id="colorFiltro" onchange="filtrarProductos()">
      <option value="">Todos los colores</option>
      <option value="Blanco">Blanco</option>
      <option value="Negro">Negro</option>
      <option value="Rosado">Rosado</option>
      <option value="Beige">Beige</option>
    </select>

  </div>


  <!-- PRODUCTOS -->
  <div class="productos" id="productos">

    <div class="producto"
      data-nombre="Zapatilla Urbana Blanca"
      data-talla="36,37,38,39"
      data-color="Blanco">

      <img src="https://images.unsplash.com/photo-1542291026-7eec264c27ff?auto=format&fit=crop&w=800&q=80">

      <div class="producto-info">
        <h3>Zapatilla Urbana Blanca</h3>
        <div class="precio">$120.000</div>
        <div class="tallas">Tallas: 36, 37, 38, 39</div>

        <button class="comprar"
          onclick="comprar('Zapatilla Urbana Blanca', '120000')">
          COMPRAR POR WHATSAPP
        </button>
      </div>
    </div>


    <div class="producto"
      data-nombre="Zapatilla Classic Negra"
      data-talla="35,36,37,38"
      data-color="Negro">

      <img src="https://images.unsplash.com/photo-1549298916-b41d501d3772?auto=format&fit=crop&w=800&q=80">

      <div class="producto-info">
        <h3>Zapatilla Classic Negra</h3>
        <div class="precio">$135.000</div>
        <div class="tallas">Tallas: 35, 36, 37, 38</div>

        <button class="comprar"
          onclick="comprar('Zapatilla Classic Negra', '135000')">
          COMPRAR POR WHATSAPP
        </button>
      </div>
    </div>


    <div class="producto"
      data-nombre="Zapatilla Rosa"
      data-talla="36,37,38"
      data-color="Rosado">

      <img src="https://images.unsplash.com/photo-1600185365483-26d7a4cc7519?auto=format&fit=crop&w=800&q=80">

      <div class="producto-info">
        <h3>Zapatilla Rosa</h3>
        <div class="precio">$145.000</div>
        <div class="tallas">Tallas: 36, 37, 38</div>

        <button class="comprar"
          onclick="comprar('Zapatilla Rosa', '145000')">
          COMPRAR POR WHATSAPP
        </button>
      </div>
    </div>


    <div class="producto"
      data-nombre="Zapatilla Beige"
      data-talla="37,38,39,40"
      data-color="Beige">

      <img src="https://images.unsplash.com/photo-1608231387042-66d1773070a5?auto=format&fit=crop&w=800&q=80">

      <div class="producto-info">
        <h3>Zapatilla Beige</h3>
        <div class="precio">$150.000</div>
        <div class="tallas">Tallas: 37, 38, 39, 40</div>

        <button class="comprar"
          onclick="comprar('Zapatilla Beige', '150000')">
          COMPRAR POR WHATSAPP
        </button>
      </div>
    </div>

  </div>

</section>


<!-- CLIENTES -->
<section class="clientes" id="clientes">

  <div class="titulo">
    <h2>⭐ CLIENTES</h2>
    <p>Lo que dicen nuestros compradores.</p>
  </div>

  <div class="comentarios">

    <div class="comentario">
      <div class="estrellas">⭐⭐⭐⭐⭐</div>
      <p>"Me encantaron las zapatillas. Muy bonitas."</p>
      <br>
      <strong>Cliente</strong>
    </div>

    <div class="comentario">
      <div class="estrellas">⭐⭐⭐⭐⭐</div>
      <p>"Excelente atención y entrega rápida."</p>
      <br>
      <strong>Cliente</strong>
    </div>

    <div class="comentario">
      <div class="estrellas">⭐⭐⭐⭐⭐</div>
      <p>"Volvería a comprar. Me gustaron mucho."</p>
      <br>
      <strong>Cliente</strong>
    </div>

  </div>

</section>


<!-- ADMIN -->
<section class="admin" id="admin">

  <div class="titulo">
    <h2>ADMINISTRACIÓN</h2>
    <p>Agrega tus nuevas zapatillas.</p>
  </div>

  <div class="admin-box">

    <label>Nombre de la zapatilla</label>
    <input type="text" id="nombre" placeholder="Ej: Zapatilla Air">

    <label>Precio</label>
    <input type="number" id="precio" placeholder="Ej: 150000">

    <label>Color</label>
    <input type="text" id="color" placeholder="Ej: Blanco">

    <label>Tallas disponibles</label>
    <input type="text" id="tallas" placeholder="Ej: 36,37,38,39">

    <label>URL de la fotografía</label>
    <input type="text" id="foto" placeholder="Pega aquí el enlace de la foto">

    <label>Descripción</label>
    <textarea id="descripcion"
      placeholder="Describe la zapatilla"></textarea>

    <button onclick="agregarProducto()">
      ➕ AGREGAR ZAPATILLA
    </button>

  </div>

</section>


<footer>
  <p>© 2026 Zapatillas M</p>
  <p>Todos los derechos reservados.</p>
</footer>


<!-- BOTÓN WHATSAPP -->
<a
  class="whatsapp"
  href="https://wa.me/573000000000"
  target="_blank">
  ☎
</a>


<script>

  /*
  ==================================================
  CAMBIA ESTE NÚMERO POR TU WHATSAPP
  ==================================================
  */

  const NUMERO_WHATSAPP = "573000000000";


  /* COMPRAR */

  function comprar(nombre, precio) {

    const mensaje =
      "Hola 👋 Estoy interesada en estas zapatillas:%0A%0A" +
      "👟 " + nombre + "%0A" +
      "💰 Precio: $" + precio + "%0A%0A" +
      "¿Está disponible?";

    window.open(
      "https://wa.me/" +
      NUMERO_WHATSAPP +
      "?text=" +
      mensaje,
      "_blank"
    );
  }


  /* FILTROS */

  function filtrarProductos() {

    const texto =
      document.getElementById("busqueda")
      .value
      .toLowerCase();

    const talla =
      document.getElementById("tallaFiltro")
      .value;

    const color =
      document.getElementById("colorFiltro")
      .value;

    const productos =
      document.querySelectorAll(".producto");


    productos.forEach(producto => {

      const nombre =
        producto.dataset.nombre.toLowerCase();

      const tallas =
        producto.dataset.talla;

      const colorProducto =
        producto.dataset.color;


      const coincideNombre =
        nombre.includes(texto);

      const coincideTalla =
        talla === "" ||
        tallas.includes(talla);

      const coincideColor =
        color === "" ||
        colorProducto === color;


      if (
        coincideNombre &&
        coincideTalla &&
        coincideColor
      ) {

        producto.style.display = "block";

      } else {

        producto.style.display = "none";

      }

    });

  }


  /* AGREGAR PRODUCTO */

  function agregarProducto() {

    const nombre =
      document.getElementById("nombre").value;

    const precio =
      document.getElementById("precio").value;

    const color =
      document.getElementById("color").value;

    const tallas =
      document.getElementById("tallas").value;

    const foto =
      document.getElementById("foto").value;

    if (
      nombre === "" ||
      precio === "" ||
      color === "" ||
      tallas === "" ||
      foto === ""
    ) {

      alert("Por favor completa todos los campos.");

      return;
    }


    const productos =
      document.getElementById("productos");


    const nuevo =
      document.createElement("div");

    nuevo.className = "producto";

    nuevo.dataset.nombre = nombre;
    nuevo.dataset.talla = tallas;
    nuevo.dataset.color = color;


    nuevo.innerHTML = `

      <img src="${foto}">

      <div class="producto-info">

        <h3>${nombre}</h3>

        <div class="precio">
          $${Number(precio).toLocaleString("es-CO")}
        </div>

        <div class="tallas">
          Tallas: ${tallas}
        </div>

        <button class="comprar"
          onclick="comprar('${nombre}', '${precio}')">

          COMPRAR POR WHATSAPP

        </button>

      </div>

    `;


    productos.appendChild(nuevo);


    alert("✅ Zapatilla agregada correctamente.");

    document.getElementById("nombre").value = "";
    document.getElementById("precio").value = "";
    document.getElementById("color").value = "";
    document.getElementById("tallas").value = "";
    document.getElementById("foto").value = "";
    document.getElementById("descripcion").value = "";

  }

</script>

</body>
</html>
