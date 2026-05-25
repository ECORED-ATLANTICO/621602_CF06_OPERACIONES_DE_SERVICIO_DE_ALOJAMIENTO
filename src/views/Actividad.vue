<template lang="pug">
  .curso-main-container.pb-3
    BannerInterno(icono="far fa-question-circle" titulo="Actividad didáctica")
    .container.tarjeta.tarjeta--blanca.p-4.p-md-5
  
      #Actividad                
        <Actividad :cuestionario="cuestionario"/>
  
  </template>

<script>
import Actividad from 'ecored-pkg-fliz/plugin/components/actividad/Actividad.vue'
export default {
  name: 'ActividadDidactica',
  components: {
    Actividad,
  },
  data: () => ({
    cuestionario: {
      tema: 'Normativa y operación hotelera: aplicando principios en recepción',
      titulo: 'Cuestionario',
      introduccion:
        '<b>Objetivo:</b> verificar la apropiación de conocimientos relacionados con normatividad hotelera, registro de huéspedes, protección de datos, seguridad de la información y responsabilidad operativa dentro de los establecimientos de alojamiento.',
      barajarPreguntas: true,
      titulo_aprobado: '¡BUEN TRABAJO!',
      titulo_reprobado: 'VUELVA A INTENTARLO',
      preguntas: [
        {
          id: 1,
          texto: '¿Cuál es la finalidad principal del registro hotelero?',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'Decorar documentos.', esCorrecta: false },
            {
              id: 'b',
              texto: 'Formalizar el ingreso del huésped.',
              esCorrecta: true,
            },
            { id: 'c', texto: 'Organizar inventarios.', esCorrecta: false },
            { id: 'd', texto: 'Promocionar servicios.', esCorrecta: false },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 2,
          texto:
            '¿Qué documentos se utiliza comúnmente para registrar huéspedes extranjeros?',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'Licencia de conducción.', esCorrecta: false },
            { id: 'b', texto: 'Tarjeta bancaria.', esCorrecta: false },
            { id: 'c', texto: 'Pasaporte vigente.', esCorrecta: true },
            { id: 'd', texto: 'Carné institucional.', esCorrecta: false },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 3,
          texto:
            '¿Cuál es uno de los principios fundamentales de la protección de datos?',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Compartir información libremente.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Confidencialidad de la información.',
              esCorrecta: true,
            },
            { id: 'c', texto: 'Publicar datos personales.', esCorrecta: false },
            {
              id: 'd',
              texto: 'Eliminar registros diariamente.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 4,
          texto:
            '¿Qué herramienta protege las redes informáticas frente a accesos no autorizados?',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'PMS.', esCorrecta: false },
            { id: 'b', texto: 'Router.', esCorrecta: false },
            { id: 'c', texto: 'Firewall.', esCorrecta: true },
            { id: 'd', texto: 'Escáner.', esCorrecta: false },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 5,
          texto: '¿Cuál es una buena práctica de ciberseguridad?',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'Compartir contraseñas.', esCorrecta: false },
            {
              id: 'b',
              texto: 'Descargar archivos desconocidos.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Utilizar contraseñas seguras.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto: 'Mantener sesiones abiertas.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 6,
          texto:
            '¿Qué información mínima debe contener el registro hotelero según la normatividad?',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Redes sociales del huésped.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Nacionalidad y fechas de estadía.',
              esCorrecta: true,
            },
            { id: 'c', texto: 'Historial médico.', esCorrecta: false },
            {
              id: 'd',
              texto: 'Información financiera completa.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 7,
          texto:
            '¿Qué área del hotel realiza principalmente el proceso de ingreso o check-in?',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'Cocina.', esCorrecta: false },
            { id: 'b', texto: 'Mantenimiento.', esCorrecta: false },
            { id: 'c', texto: 'Recepción.', esCorrecta: true },
            { id: 'd', texto: 'Compras.', esCorrecta: false },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 8,
          texto: '¿Cuál es el propósito de las copias de seguridad?',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Decorar archivos digitales.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Recuperar información en caso de pérdida.',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto: 'Eliminar datos automáticamente.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Compartir información públicamente.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 9,
          texto: '¿Qué significa la sigla ESCNNA?',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Estrategia de control hotelero.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Sistema estadístico nacional.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Explotación sexual comercial de niños, niñas y adolescentes.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto: 'Escuela de seguridad turística.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 10,
          texto: '¿Qué acción debe realizarse ante un correo sospechoso?',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'Abrirlo inmediatamente.', esCorrecta: false },
            {
              id: 'b',
              texto: 'Descargar archivos adjuntos.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Compartirlo con otros usuarios.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Verificar su autenticidad antes de abrirlo.',
              esCorrecta: true,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
      ],
      mensaje_final_aprobado: '¡Excelente! Ha superado la actividad.',
      mensaje_final_reprobado:
        'Le recomendamos volver a revisar el componente formativo e intentar nuevamente la actividad didáctica.',
    },
  }),
}
</script>
