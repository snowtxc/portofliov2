<template>
  <div class="flex flex-col h-full">
    <div class="flex flex-col items-center justify-center justify-items-center m-auto">
        <img class="inline object-cover w-24 h-24 mr-2 rounded-full bg-white" :src="mainPhoto"/>
        <h1 class="my-5 text-lg font-bold">Hola, Soy Rodrigo 👋</h1>
        <h1 class="my-5 text-4xl md:text-5xl lg:text-6xl lg:px-32 xl:px-56 tracking-tighter leading-tight md:leading-none text-center font-bold">
          Tecnólogo Informatico, Full Stack Developer VUE JS, PHP <span class="italic"></span></h1>
        <p class="my-5 mb-10 text-sm xl:text-lg md:text-md tracking-tight md:px-12 lg:px-30 text-center font-semibold text-theme-secondary">
          Desarrollador de software con experiencia en diversas tecnologías y lenguajes de programación,principalmente utilizando Vue JS y PHP con Laravel y Codeigniter.
        </p>
        <Button class="mb-16" cta='Contactame' />

        <!-- Cards -->
        <div id="cards" class="my-5">
          <h1 class="text-center md:text-xl font-medium tracking-tight leading-tight text-md mb-5">
              Algunos Proyectos<br class="hidden md:block">
          </h1>

          <div class="flex flex-col md:flex-col lg:px-32 w-full">
              <div class="block md:mr-5">
                <sequential-entrance fromLeft delay="2000"><Card :cardData="cardData1" /></sequential-entrance>
                <sequential-entrance fromTop delay="2000"><Card :cardData="cardData2" /></sequential-entrance>
              </div>

              <div class="block md:mr-5">
                <sequential-entrance fromRight delay="2000"><Card :cardData="cardData3" /></sequential-entrance>
                <sequential-entrance fromBottom delay="4000"><Card :cardData="cardData4" /></sequential-entrance>
              </div>
          </div>
        </div>


        <Button class="mb-16" cta='Contactame' />

        <hr class="my-10 w-full border-theme-tertiary border-dashed">


    </div>

  </div>
</template>

<script>
import { ChevronsDownIcon } from 'vue-feather-icons'

import mainPhoto from '~/assets/images/yo.jpeg'
import cardImage1 from '~/assets/images/scadasystem.png'
import cardImage2 from '~/assets/images/satweb.png'
import cardImage3 from '~/assets/images/learndo.png'
import cardImage4 from '~/assets/images/blackhawk.png'

export default {
  data() {
      return {
        title: 'Home',
        mainPhoto: mainPhoto,
        cardData1: {
          tecnologies: ["PHP" , "Vue Js" , "Laravel" , "MySql", "Tailwind CSS"],
          photo: cardImage1,
          title: "Satweb",
          body: `Desarrollé junto a mi equipo un Sistema de tipo SCADA (Supervisory Control and Data Acquisition) que permitió monitorizar dispositivos en tiempo real. Utilizamos  Vue.js y Laravel para el frontend y backend respectivamente, junto con Laravel Websockets para la comunicación en tiempo real. La arquitectura a grandes razgos incluía un servidor FTP donde se publicaban archivos XML con la respectiva información
          de los dispositivos, luego nuestro backend consumía estos archivos para generar historicos y transmitirlos en tiempo real mediante websockets a nuestro frontend.Este proyecto se realizo en el marco del proyecto final de Carrera.
          `
        },
        cardData2: {
          tecnologies: ["PHP" , "Vue Js" , "Codeingiter" , "MySql", "Quasar"],
          photo: cardImage2,
          title: `
                  SatWeb
                `,
          body: `Producto comercial  para Empresas de Asistencia Técnica y Mantenimiento.Este sistema permite permite gestionar un servicio técnico desde cualquier lugar y dispositivo. Administrar las sucursales de su taller y recepcion equipos
          `
        },
        cardData3: {
          tecnologies: ["Vue Js", "Firebase", "Firestore","Quasar"],
          photo: cardImage4,
          title: `
            Sistema Defensa BlackHawk
          `,
          body: `
            What direction is your product taking? How do you plan to handle
            uncertainty? Learn simple steps to avoid the dilemma of build-trap
            and navigate from a project to a product.
          `
        },
        cardData4: {
          tecnologies: ["Next", "Laravel", "MySql" , "Firebase", "Tailwind CSS"],
          photo: cardImage3,
          title: `
          Learn DO
          `,
          body: `
            Junto a mi equipo desarrollamos una plataforma de aprendizaje Online(E-Learning) en el marco de la asignatura "Taller de PHP" de la carrera.El Sistema fue desarrollado utilizando
            Php con Laravel y el frontend fue construido en React con Next.Sus principales funcionalidades incluyen comprar cursos utilizando Paypal, envio automatico de recordatorios ,visualización del progreso, realización de evaluaciones por cada sección del curso.El sistema contaba con 2 Roles Distintos(Estudiante y Profesor)
          `
        },
      }
  },

  components: {
    ChevronsDownIcon
  }
}
</script>
