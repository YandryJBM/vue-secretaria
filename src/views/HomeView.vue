<script>
import { RouterLink } from "vue-router";
</script>

<template>
  <header>
  
    <div class="texts">
      <h1 class="hero__title">Tus Tramites Desde La Comodidad De Tu Casa.</h1>
            <p class="hero__paragraph">Te Facilitamos Tus Tramites.</p>
           <section class="buttons">
            <router-link class="buttons__btn buttons__btn--login" to="/login"
           >Inicia Sesion</router-link>
           <router-link class="buttons__btn buttons__btn--register" to="/register"
           >Registrate</router-link>
           <router-link class="buttons__btn buttons__btn--Contactanos" to="/contacto"
           >Contactanos</router-link>
          </section>
    </div>
  </header>
  <main>
        <section class="container about">
            <h4 class="subtitle">Sobre Nosotros</h4>
            <p> Nuestro objetivo se basa en facilitar todos aqquellos tramites personales que debeas hacer en tu facultad o la universidad Desde
                la comodidad de tu casa, asi de mas usas en los cuales puedes tener mas informacion precisa de cuales son lso requisitos que vas
                a necesitar a lo largo de tu tramite.</p>
            <div class="about__main">
                <article class="about__icons">
                    <img src="../assets/guardar.png" class="about__icon">
                    <h3 class="about__title">Fácil de utilizar</h3>
                    <p class="about__paragrah">Descarga y sube documentes en los formatos mas accesibles como pdf y word.</p>
                </article>

                <article class="about__icons">
                    <img src="../assets/notificacion.png" class="about__icon">
                    <h3 class="about__title">Notificaciones</h3>
                    <p class="about__paragrah">Te notificará las nuevas actualizaciones mediante correo. </p>
                </article>
                <br>
            </div>
            <footer class="footer">
        <section class="footer__copy container">
            <div class="footer__social">
                <a href="https://www.facebook.com/Facci.Uleam/">
                <img src="../assets/facebook.svg" class="footer__img">
                </a>
                <a href="https://twitter.com/facciuleam">
                <img src="../assets/twitter.svg" class="footer__img">
                </a>
                <a href="https://www.youtube.com/channel/UCOferC0PjpEUegrVq8Re-TQ">
                <img src="../assets/youtube.svg" class="footer__img">
                </a>
            </div>
            <h3 class="footer__copyright">Derechos reservados 2022 &copy; Secretaría Virtual</h3>
        </section>
  </footer>
        </section>
    </main>
</template>

<style scoped>
header {
  width: 100%;
  height: 750px;
  background-image: url(../assets/indexbiblioteca.png);
  background-attachment: fixed;
  background-size: cover;
  background-position: center;
  overflow: hidden;
  color: #fff;
  text-align: center;
  margin-bottom: 50px;
}

.texts {
  height: 100%;
  display: flex;
  flex-direction: column;
  justify-content: center;
}

.texts__title {
  font-size: 3.5rem;
  text-shadow: 2px  1px 2px black,
             1px  1px 1px black,
            -2px  1px 2px black,
             2px -1px 2px black;
}

.buttons {
  display: flex;
  justify-content: space-evenly;
  
}

.buttons__btn {
  text-decoration: none;
  padding: 1.3em 3em;
  font-weight: bold;
  text-transform: uppercase;
  letter-spacing: 2px;
  color: #fff;
  background-color: #282828;
  border: none;
  border-radius: 45px;
  box-shadow: 0px 8px 15px rgba(0, 0, 0, 0.1);
  transition: all 0.3s ease 0s;
  cursor: pointer;
  outline: none;
}

.buttons__btn--login:hover {
  background-color: #18db28;
  box-shadow: 0px 15px 20px rgba(41, 207, 141, 0.4);
  transform: translateY(-7px);
}

.buttons__btn--Contactanos:hover {
  background-color: #fa1818;
  box-shadow: 0px 15px 20px rgba(229, 46, 46, 0.4);
  transform: translateY(-7px);
}

.buttons__btn--register:hover {
  background-color: #f5df1d;
  box-shadow: 0px 15px 20px rgba(229, 46, 46, 0.4);
  transform: translateY(-7px);
}

.buttons__btn:active {
  transform: translateY(-1px);
}

.nav__title {
  font-size: 40px;
  font-weight: bold;
  color: #fff;
  text-decoration: none;
  text-align:center;
  font-weight: 700;
  text-shadow: 2px  1px 2px black,
             1px  1px 1px black,
            -2px  1px 2px black,
             2px -1px 2px black;
}

.container {
    width: 90%;
    max-width: 1200px;
    margin: 0 auto;
    overflow: hidden;
    padding: var(--padding-container);
}

.about {
    text-align: center;
}

.footer__copyright {
    font-weight: 300;
}

.footer {
    background-color: #4a2277;
}

.footer__copy {
    --padding-container: 30px 0;
    text-align: center;
    color: #fff;
}

.footer__img {
    width: 30px;
}

.hero__paragraph {
    margin-bottom: 5px;
    margin-top: 10px;
}


.hero__container {
    max-width: 800px;
    --padding-container: 0;
    display: grid;
    grid-auto-rows: max-content;
    align-content: center;
    gap: 2em;
    padding-bottom: 50px;
    text-align: center;
}


.hero__title {
    font-size: 3rem;
}

.cta {
    display: inline-block;
    background-color: #7b9977;
    justify-self: center;
    color: #fff;
    text-decoration: none;
    padding: 13px 30px;
    border-radius: 32px;
}
</style>
