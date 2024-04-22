<template>
    <div class="accordion flex flex-col">
        <!--  Panel 1  -->
        <div class="w-full">
            <input type="checkbox" name="panel" id="panel-1" class="hidden">
            <label for="panel-1" class="relative block bg-black text-white p-4 shadow border-b border-grey">¿Cual es tu formación?</label>
            <div class="accordion__content overflow-hidden bg-grey-lighter">
                <h2 class="accordion__header font-medium pt-4 pl-4">Mi formación</h2>
                <p class="accordion__body p-4">
                  Mis inicios fueron cuando tenía 16 años y realicé la secundaria en un curso orientado a informática en UTU (Uruguay), esto me garantizó una sólida base de conocimientos sobre programación, bases de datos, sistemas operativos y más.
                </p>
                <p class="accordion__body p-4">
                  Luego me gradué de una carrera de 3 años llamada "Tecnólogo en Informática" en UTEC (Uruguay), donde principalmente trabajé en múltiples talleres de distintas tecnologías como PHP, .NET. A su vez, desarrollé un pensamiento analítico, aprendí sobre ingeniería de software, redes, sistemas operativos y mucho más. Considero que fue una carrera orientada en su mayoría a la práctica constante y al enfrentamiento de problemas del mundo real.

                </p>

            </div>
        </div>
        <!-- Panel 2 -->
        <div class="w-full">
            <input type="checkbox" name="panel" id="panel-2" class="hidden">
            <label for="panel-2" class="relative block bg-black text-white p-4 shadow border-b border-grey">¿Cuál es tu experiencia profesional?</label>
            <div class="accordion__content overflow-hidden bg-grey-lighter">

                <h2 class="accordion__header font-medium pt-4 pl-4">Experiencia Profesional</h2>
                <p class="accordion__body p-4">
                    Trabajo desde agosto 2022 en el rubro como Sofware Developer. Me he desempeñado en la implementación de nuevas funcionalidades en distintos proyectos principalmene utilizando  el stack Vue Js y PHP, así como diseño de base de datos relacionales y no relacionales como Firestore, correción de bugs detectados, migración de sistemas legados, ánalisis y relevamiento de requerimientos
                </p>
                <p class="accordion__body p-4">
                    He trabajado en proyectos de uso comercial para público en general como un software de gestión de equipos técnicos, software a medida para gestión de una empresa de seguridad chilena, así como
                    software interno de la empresa para el manejo de tickets y reclamos de Normas ISO.
                </p>

            </div>
        </div>
        <!--  Panel 3  -->
        <div class="w-full">
            <input type="checkbox" name="panel" id="panel-3" class="hidden">
            <label for="panel-3" class="relative block bg-black text-white p-4 shadow border-b border-grey">¿Cuáles son tus habilidades clave?</label>
            <div class="accordion__content overflow-hidden bg-grey-lighter">
                <h2 class="accordion__header font-medium pt-4 pl-4">Habilidades Claves</h2>
                <p class="accordion__body p-4">
                    Mis habilidades técnicas principalmente se centran en desarrollo y mantenimiento de Software con PHP y Vue JS,así como conocimientos de base de datos SQL y no SQL, control de versiones con GIT.
                    A nivel académico he trabajado con otras tecnólogias como React, .NET, Java, C++ y más.
                </p>
            </div>
        </div>
        <!--  Panel 4  -->
        <div class="w-full">
            <input type="checkbox" name="panel" id="panel-4" class="hidden">
            <label for="panel-4" class="relative block bg-black text-white p-4 shadow border-b border-grey">¿Cómo pueden contactarte?</label>
            <div class="accordion__content overflow-hidden bg-grey-lighter">
                <h2 class="accordion__header font-medium pt-4 pl-4">Contacto</h2>
                <p class="accordion__body p-4">
                    Mi correo es rodrigo.castro.v23@gmail.com y mi número de celular 092365856. Estaré encantado de charlar por cualquier interés 😁
                </p>

            </div>
        </div>

        <div class="w-full">
            <input type="checkbox" name="panel" id="panel-5" class="hidden">
            <label for="panel-5" class="relative block bg-black text-white p-4 shadow border-b border-grey">¿Qué tipo de proyectos te interesan?</label>
            <div class="accordion__content overflow-hidden bg-grey-lighter">
                <p class="accordion__body p-4">
                  Puedo adaptarme a trabajar en cualquier proyecto, mi experiencia viene más por el desarrollo web pero siempre me gusta innovar y enfrentarme a nuevos desafíos que supongan un reto para mi 💪, y a su vez ayude a alcanzar los intereses de una empresa
                </p>

            </div>
        </div>

    </div>
</template>

<style>
    label:after {
    content: '+';
    position: absolute;
    right: 1em;
    color: #fff;
    }

    input:checked + label:after {
    content: '-';
    line-height: .8em;
    }

    .accordion__content{
    max-height: 0em;
    transition: all 0.4s cubic-bezier(0.865, 0.14, 0.095, 0.87);
    }
    input[name='panel']:checked ~ .accordion__content {
    /* Get this as close to what height you expect */
    max-height: 50em;
    }
</style>
