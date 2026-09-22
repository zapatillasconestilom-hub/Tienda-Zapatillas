<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <title>ZAPPI | Tienda de Zapatillas</title>

  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: Arial, sans-serif;
    }

    body {
      background: #f5f5f5;
      color: #111;
    }

    header {
      background: #111;
      color: white;
      padding: 20px 8%;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }

    .logo {
      font-size: 28px;
      font-weight: bold;
      letter-spacing: 2px;
    }

    nav a {
      color: white;
      text-decoration: none;
      margin-left: 20px;
    }

    .principal {
      min-height: 420px;
      background: white;
      display: flex;
      justify-content: center;
      align-items: center;
      text-align: center;
      padding: 40px 20px;
    }

    .principal h1 {
      font-size: 48px;
      margin-bottom: 15px;
    }

    .principal p {
      font-size: 20px;
      margin-bottom: 25px;
      color: #555;
    }

    .boton {
      display: inline-block;
      background: #111;
      color: white;
      padding: 14px 28px;
      border-radius: 30px;
      text-decoration: none;
      font-weight: bold;
    }

    section {
      padding: 50px 8%;
    }

    .titulo {
      text-align: center;
      margin-bottom: 35px;
      font-size: 32px;
    }

    .productos {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
      gap: 25px;
    }

    .producto {
      background: white;
      border-radius: 15px;
      overflow: hidden;
      box-shadow: 0 4px 15px rgba(0,0,0,0.08);
      text-align: center;
      padding-bottom: 20px;
    }

    .producto img {
      width: 100%;
      height: 240px;
      object-fit: cover;
      background: #ddd;
    }

    .producto h3 {
      margin: 15px 0 8px;
    }

    .precio {
      font-size: 20px;
      font-weight: bold;
      margin-bottom: 15px;
    }

    .comprar {
      display: inline-block;
      background: #111;
      color: white;
      padding: 10px 20px;
      border-radius: 20px;
      text-decoration: none;
    }

    .comentarios {
      background: white;
      border-radius: 15px;
      padding: 30px;
      max-width: 800px;
      margin: auto;
      text-align: center;
    }

    .comentarios p {
      margin: 15px 0;
      color: #555;
    }

    footer {
      background: #111;
      color: white;
      text-align: center;
      padding: 30px;
    }

    @media (max-width: 600px) {
      header {
        flex-direction: column;
        gap: 15px;
      }

      .principal h1 {
        font-size: 36px;
      }

      nav a {
        margin: 5px;
      }
    }
  </style>
</head>

<body>

  <!-- ENCABEZADO -->
  <header>
    <div class="logo">ZAPPI</div>

    <nav>
      <a href="#inicio">Inicio</a>
      <a href="#productos">Zapatillas</a>
      <a href="#comentarios">Opiniones</a>
      <a href="#contacto">Contacto</a>
    </nav>
  </header>


  <!-- INICIO -->
  <section class="principal" id="inicio">
    <div>
      <h1>NUEVA COLECCIÓN</h1>

      <p>
        Zapatillas modernas para todos tus estilos.
      </p>

      <a href="#productos" class="boton">
        VER ZAPATILLAS
      </a>
    </div>
  </section>


  <!-- PRODUCTOS -->
  <section id="productos">

    <h2 class="titulo">
      Zapatillas destacadas
    </h2>

    <div class="productos">

      <!-- PRODUCTO 1 -->
      <div class="producto">

        <img
          src="https://images.unsplash.com/photo-1542291026-7eec264c27ff?w=800"
          alt="Zapatillas deportivas"
        >

        <h3>Urban Classic</h3>

        <div class="precio">
          $149.900
        </div>

        <a
          class="comprar"
          href="https://wa.me/573000000000"
          target="_blank"
        >
          Comprar
        </a>

      </div>


      <!-- PRODUCTO 2 -->
      <div class="producto">

        <img
          src="https://images.unsplash.com/photo-1549298916-b41d501d3772?w=800"
          alt="Zapatillas blancas"
        >

        <h3>Street White</h3>

        <div class="precio">
          $169.900
        </div>

        <a
          class="comprar"
          href="https://wa.me/573000000000"
          target="_blank"
        >
          Comprar
        </a>

      </div>


      <!-- PRODUCTO 3 -->
      <div class="producto">

        <img
          src="https://images.unsplash.com/photo-1552346154-21d32810aba3?w=800"
          alt="Zapatillas deportivas"
        >

        <h3>Sport Max</h3>

        <div class="precio">
          $189.900
        </div>

        <a
          class="comprar"
          href="https://wa.me/573000000000"
          target="_blank"
        >
          Comprar
        </a>

      </div>


      <!-- PRODUCTO 4 -->
      <div class="producto">

        <img
          src="https://images.unsplash.com/photo-1460353581641-37baddab0fa2?w=800"
          alt="Zapatillas modernas"
        >

        <h3>Trend Black</h3>

        <div class="precio">
          $179.900
        </div>

        <a
          class="comprar"
          href="https://wa.me/573000000000"
          target="_blank"
        >
          Comprar
        </a>

      </div>

    </div>
  </section>


  <!-- OPINIONES -->
  <section id="comentarios">

    <h2 class="titulo">
      Lo que dicen nuestros clientes
    </h2>

    <div class="comentarios">

      <p>⭐⭐⭐⭐⭐</p>

      <p>
        "Me encantaron mis zapatillas. Muy bonitas y cómodas."
      </p>

      <p>
        — Cliente ZAPPI
      </p>

    </div>

  </section>


  <!-- CONTACTO -->
  <section id="contacto">

    <h2 class="titulo">
      ¿Quieres comprar?
    </h2>

    <div style="text-align:center;">

      <p style="margin-bottom:20px;">
        Escríbenos por WhatsApp para consultar tallas,
        colores y disponibilidad.
      </p>

      <a
        class="boton"
        href="https://wa.me/573000000000"
        target="_blank"
      >
        ESCRIBIR POR WHATSAPP
      </a>

    </div>

  </section>


  <!-- PIE DE PÁGINA -->
  <footer>

    <p>
      © 2026 ZAPPI - Tienda de Zapatillas
    </p>

    <p style="margin-top:10px;">
      Síguenos en nuestras redes sociales
    </p>

  </footer>

</body>
</html>
🟢 PASO 7: Guardar

Después de pegar todo el código:

Baja hasta el final de la página.
