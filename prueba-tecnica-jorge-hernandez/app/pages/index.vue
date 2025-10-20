<template>
  <header>
    <nav id="navbar" class="navbar">
      <div class="navbar__container">
        <a href="#" class="navbar__logo">JH</a>
        <div class="navbar__links">
          <a href="#hero" class="navbar__link">Inicio</a>
          <a href="#about" class="navbar__link">Acerca de mí</a>
          <a href="#technologies" class="navbar__link">Tecnologías</a>
          <a href="#experience" class="navbar__link">Experiencia</a>
          <a href="#projects" class="navbar__link">Proyectos</a>
          <a href="#contact" class="navbar__link">Contacto</a>
        </div>
        <div class="navbar__icons">
          <!-- Iconos SVG de GitHub y LinkedIn -->
           <a class="footer__link" href="#">
          <!-- Icono GitHub -->
          <svg
            class="icon"
            fill="none"
            height="24"
            stroke="currentColor"
            stroke-linecap="round"
            stroke-linejoin="round"
            stroke-width="2"
            viewBox="0 0 24 24"
            width="24"
          >
            <path
              d="M9 19c-5 1.5-5-2.5-7-3m14 6v-3.87a3.37 3.37 0 0 0-.94-2.61c3.14-.35 6.44-1.54 6.44-7A5.44 5.44 0 0 0 20 4.77..."
            ></path>
          </svg>
        </a>
        <a class="footer__link" href="#">
          <!-- Icono LinkedIn -->
          <svg
            class="icon"
            fill="none"
            height="24"
            stroke="currentColor"
            stroke-linecap="round"
            stroke-linejoin="round"
            stroke-width="2"
            viewBox="0 0 24 24"
            width="24"
          >
            <path d="M16 8a6 6 0 0 1 6 6v7h-4v-7a2 2 0 0 0-2-2..."></path>
            <rect height="12" width="4" x="2" y="9"></rect>
            <circle cx="4" cy="4" r="2"></circle>
          </svg>
        </a>
      </div>
    
      </div>
    </nav>
  </header>

  <main>
    <section class="hero" id="hero">
      <div class="hero__container">
        <div class="photo__placeholder">
          <span class="hero__photo">Espacio para foto</span>
        </div>
        <div>
          <h1 class="hero__title">Jorge Hernández</h1>
          <p class="hero__subtitle">
            Desarrollador Web Junior apasionado por crear aplicaciones web
            responsivas y fáciles de usar.
          </p>
          <p class="hero__description">
            Tengo conocimientos en tecnologías web modernas, incluyendo HTML,
            CSS y JavaScript, con experiencia práctica en la construcción de
            interfaces dinámicas con React y backends robustos con Node.js.
            Estoy buscando activamente oportunidades para contribuir a proyectos
            innovadores y hacer crecer mis habilidades dentro de un entorno de
            equipo colaborativo y dinámico.
          </p>
          <a class="hero__button" href="#about"> Ver Perfil Completo </a>
        </div>
      </div>
    </section>

    <section class="hero" id="about">
     <div class="">
        <h2 class="hero__title">Acerca de mí</h2>
        <div class="">
            <h3 class="hero__subtitle">Jorge Hernández</h3>
            <p class="hero__description">
              Soy un desarrollador web junior apasionado por crear aplicaciones
              web innovadoras y fáciles de usar. Mi viaje al mundo del
              desarrollo web comenzó con una fascinación por cómo funcionan los
              sitios web, y desde entonces me he enganchado. Estoy ansioso por
              contribuir con mis habilidades y entusiasmo a un equipo dinámico,
              donde pueda continuar aprendiendo y creciendo como desarrollador.
            </p>
            <h4 class="hero__subtitle">Intereses</h4>
            <p class="hero__description">
              Más allá de la codificación, estoy profundamente interesado en
              tecnologías emergentes como la IA y blockchain. Disfruto
              explorando sus posibles aplicaciones y manteniéndome actualizado
              con los últimos avances. También tengo un gran interés en el
              diseño UI/UX, esforzándome por crear interfaces intuitivas y
              visualmente atractivas que mejoren la experiencia del usuario.
            </p>
            <a class="hero__button" href="#projects"> Ver Mis Proyectos </a>
          </div>
          </div>
    </section>


    <!-- Pasar a grid -->
    <section class="technologies" id="technologies">
        <div>
        <h2 class="technologies__title">Tecnologías que uso</h2>
         <div class="technologies__container">
          <div class="">
            <p class="">HTML</p>
          </div>
          <div class="">
            <p class="">CSS</p>
          </div>
          <div class="">
            <p class="">JavaScript</p>
          </div>

          <div class="">
            <p class="">SQL</p>
          </div>

          <div class="">
            <p class="">Git</p>
          </div>
        </div>
        </div>
      
    </section>

    <section class="hero" id="experience">
      <div class="">
        <h2 class="hero__title">Experiencia Laboral</h2>
        <div class="">
          <div class="">
            <div class="hero">
              <div class="hero__photo"></div>
              <div class="">
                <p class="hero__description">Enero 2023 - Presente</p>
                <h3 class="hero__subtitle">Desarrollador Web Junior</h3>
                <p class="hero__subtitle">Empresa Innovadora S.A.</p>
                <p class="hero__description">
                  Desarrollo y mantenimiento de aplicaciones web utilizando
                  React y Node.js. Colaboración en el diseño de interfaces de
                  usuario y optimización del rendimiento.
                </p>
              </div>
            </div>
            <div class="hero">
              <div class="hero__photo"></div>
              <div class="">
                <p class="hero__description">Junio 2022 - Diciembre 2022</p>
                <h3 class="hero__subtitle">Pasante de Desarrollo Frontend</h3>
                <p class="hero__subtitle">Tech Solutions Co.</p>
                <p class="hero__descripition">
                  Asistencia en la creación de componentes de UI con HTML, CSS y
                  JavaScript. Participación en pruebas y depuración de código.
                </p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <section class="projects" id="projects">
      <div class="">
        <h2 class="projects__title">Proyectos</h2>
        <div class="projects__container">
          
          <div class="">
            <img
              alt="Laptop con código en la pantalla"
              class="hero__photo"
              src="https://lh3.googleusercontent.com/aida-public/AB6AXuATFLCKcf_mTlx0krNNBqtvAORIS8t0Jvho9d7ltsqSK-R5MUtlBJEQTEL9vDUPMVoPM9UW2hOpTO7Qw5vY2Ia5mvNnAjM4wx4TLqGOTex6esV4vJKYQfEyNcauY5BEcxDowcs1CTQnCWJDK8NGiVcELu7hV32DbYeyoIj1jLmyRg6oMOpKjg8zp8QOn4N3ovtcfYS1EC567O_NtfoqkkuH3qdOI5IYb-FcIvems4uL4jyznmo486VPlBUI32Iujoa8m6syzsTr0dY8"
            />
            <h3 class="hero__subtitle">Proyecto 1</h3>
            <p class="hero___description">
              Una breve descripción de este increíble proyecto que muestra mis
              habilidades y creatividad.
            </p>
            <a class="hero__button">Ver más</a>
          </div>

          <div class="">
            <img
              alt="Código en un monitor oscuro"
              class="hero__photo"
              src="https://lh3.googleusercontent.com/aida-public/AB6AXuC_m1e7-17v6k41tU1LWduGbY2Yt3vLHfd2us_Gy7-lfBAt8km2N1HEU_ZssaxzdK3-aWEmkI4RntZVK9ar5N01YhL3aFbPS6ais0OCORuXvFCAOm9Usc3EacKtGEsnoWadD__b2_8Q0cbfXZI2MJtH1xab7oL-g5BtUTWzvn8YovpsvHGj-kLgT5dl2Cs5woxvy_-B9JaNEz-JY-wnf59hUcQuDG_12o5rLrOUAinpmszlBjDqNIph0bJ3b6mwSrKiriNEHuiz7qh1"
            />
            <h3 class="hero__subtitle">Proyecto 2</h3>
            <p class="hero__description">
              Otro proyecto interesante que demuestra mi capacidad para resolver
              problemas y construir soluciones.
            </p>
            <a class="hero__button" href="#">Ver más</a>
          </div>

          <div class="bg-card-dark rounded-lg shadow-lg overflow-hidden">
            <img
              alt="Escritorio con laptop, monitor y café"
              class="hero__photo"
              src="https://lh3.googleusercontent.com/aida-public/AB6AXuDEuOM5yFTFhYNe_Z_0OtrFJrnfnwOMH2PyPSKuG8MZI3b9HMC22gMQhw48JWtfxbEHVuJt6FWOowaL1tvWxkN76S3KTmX1HnXXkbbOieqx3wjjQzO5uQVEXmf-zom6ASqUkqSzTQf9WohxqZzgPiGsyF3fi-Y5loxUhGnmLTIS61YyyMGJ65QKRFM7nVBEsTwjDcZUx2vu0PFONK9GcSb5ixtD3qdOmmYMUwHuBAUOI0gFu4lI0InHqKqNx5gudK4lStumQsuPhchq"
            />
            <h3 class="hero__subtitle">Proyecto 3</h3>
            <p class="hero__description">
              Un proyecto desafiante que me permitió crecer como desarrollador y
              aprender nuevas tecnologías.
            </p>
            <a class="hero__button" href="#">Ver más</a>
          </div>
        </div>
      </div>
    </section>

    <section class="hero" id="contact">
      <div class="">
        <h2 class="hero__title">Contacto</h2>
        <p class="hero__description">
          Siempre estoy abierto a discutir nuevos proyectos, ideas creativas u
          oportunidades para ser parte de tus visiones. ¡No dudes en
          contactarme!
        </p>
        <form action="#" class="">
          <div>
            <label class="" for="name">Nombre</label>
            <input
              class=""
              id="name"
              name="name"
              placeholder="Tu Nombre"
              type="text"
            />
          </div>
          <div>
            <label class="" for="email">Correo electrónico</label>
            <input
              class=""
              id="email"
              name="email"
              placeholder="Tu Correo Electrónico"
              type="email"
            />
          </div>
          <div>
            <label class="" for="message">Mensaje</label>
            <textarea
              class=""
              id="message"
              name="message"
              placeholder="Tu Mensaje"
              rows="4"
            ></textarea>
          </div>
          <div class="">
            <button class="hero__button" type="submit">Enviar Mensaje</button>
          </div>
        </form>
      </div>
    </section>
  </main>

  <footer class="footer">
    <div class="footer__container">
      <p>© 2024 Jorge Hernández. Todos los derechos reservados.</p>
      <div class="footer__social">
        <a class="footer__link" href="#">
          <!-- Icono GitHub -->
          <svg
            class="icon"
            fill="none"
            height="24"
            stroke="currentColor"
            stroke-linecap="round"
            stroke-linejoin="round"
            stroke-width="2"
            viewBox="0 0 24 24"
            width="24"
          >
            <path
              d="M9 19c-5 1.5-5-2.5-7-3m14 6v-3.87a3.37 3.37 0 0 0-.94-2.61c3.14-.35 6.44-1.54 6.44-7A5.44 5.44 0 0 0 20 4.77..."
            ></path>
          </svg>
        </a>
        <a class="footer__link" href="#">
          <!-- Icono LinkedIn -->
          <svg
            class="icon"
            fill="none"
            height="24"
            stroke="currentColor"
            stroke-linecap="round"
            stroke-linejoin="round"
            stroke-width="2"
            viewBox="0 0 24 24"
            width="24"
          >
            <path d="M16 8a6 6 0 0 1 6 6v7h-4v-7a2 2 0 0 0-2-2..."></path>
            <rect height="12" width="4" x="2" y="9"></rect>
            <circle cx="4" cy="4" r="2"></circle>
          </svg>
        </a>
      </div>
    </div>
  </footer>
</template>
