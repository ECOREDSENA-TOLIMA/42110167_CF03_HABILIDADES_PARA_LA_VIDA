<template lang="pug">
  .curso-main-container.pb-3
    BannerInterno(icono="far fa-question-circle" titulo="Actividad didáctica")
    .container.tarjeta.tarjeta--blanca.p-4.p-md-5
  
      #Actividad                
        <Actividad :cuestionario="cuestionario"/>
  
  </template>

<script>
export default {
  name: 'ActividadDidactica',
  data: () => ({
    cuestionario: {
      tema: 'Conociendo las competencias socioemocionales (CSE).',
      titulo: 'Cuestionario',
      introduccion:
        '<b> Objetivo:</b> identificar las competencias socioemocionales (CSE) del ser, basado en la transformación social que puede lograr alcanzar en sus procesos de vida.<br><b>Se desarrollará una actividad tipo evaluación, con ítems de falso o verdadero; así como, de opción múltiple con única respuesta.</b>',
      barajarPreguntas: true,
      preguntas: [
        {
          id: 1,
          texto:
            'El marco lógico solo sirve para proyectos con financiamiento.',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'Verdadero', esCorrecta: false },
            { id: 'b', texto: 'Falso', esCorrecta: true },
          ],
          mensaje_correcto:
            'El marco lógico es útil tanto para proyectos con o sin financiamiento, ya que estructura objetivos y acciones.',
          mensaje_incorrecto:
            '¡No se preocupe por el error! Cada respuesta es una oportunidad para aprender y mejorar. Lo importante es seguir adelante y fortalecer los conocimientos. ',
        },
        {
          id: 2,
          texto:
            'La agencia permite a las comunidades tomar decisiones enfocadas en el bienestar común.',
          imagen: require('@/assets/actividad/imagen2.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'Verdadero', esCorrecta: true },
            { id: 'b', texto: 'Falso', esCorrecta: false },
          ],
          mensaje_correcto:
            'La agencia facilita la acción colectiva hacia objetivos compartidos y sostenibles.',
          mensaje_incorrecto:
            '¡Continúe no se rinda! Equivocarse es aprender. Siga intentando, está en el camino correcto.',
        },
        {
          id: 3,
          texto:
            'Las competencias socioemocionales no son necesarias para la ciudadanía activa.',
          imagen: require('@/assets/actividad/imagen3.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'Verdadero', esCorrecta: false },
            { id: 'b', texto: 'Falso', esCorrecta: true },
          ],
          mensaje_correcto:
            'Las competencias socioemocionales son fundamentales para interactuar de forma constructiva en sociedad.',
          mensaje_incorrecto:
            '¡No se preocupe por el error! Cada respuesta es una oportunidad para aprender y mejorar. Lo importante es seguir adelante y fortalecer los conocimientos. ',
        },
        {
          id: 4,
          texto:
            'El espacio público está relacionado con la interacción individual, sin dimensión colectiva.',
          imagen: require('@/assets/actividad/imagen4.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'Verdadero', esCorrecta: false },
            { id: 'b', texto: 'Falso', esCorrecta: true },
          ],
          mensaje_correcto:
            'El espacio público se caracteriza por la dimensión colectiva e intereses comunes.',
          mensaje_incorrecto:
            '¡Continúe no se rinda! Equivocarse es aprender. Siga intentando, está en el camino correcto.',
        },
        {
          id: 5,
          texto:
            'El objetivo general en el marco lógico describe el impacto deseado a largo plazo.',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'Verdadero', esCorrecta: true },
            { id: 'b', texto: 'Falso', esCorrecta: false },
          ],
          mensaje_correcto:
            'Este objetivo guía todas las acciones hacia un cambio significativo en la comunidad.',
          mensaje_incorrecto:
            '¡No se preocupe por el error! Cada respuesta es una oportunidad para aprender y mejorar. Lo importante es seguir adelante y fortalecer los conocimientos. ',
        },
        {
          id: 6,
          texto:
            'La agencia adaptativa permite a las personas planificar metas a largo plazo.',
          imagen: require('@/assets/actividad/imagen2.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'Verdadero', esCorrecta: false },
            { id: 'b', texto: 'Falso', esCorrecta: true },
          ],
          mensaje_correcto:
            'La agencia adaptativa se enfoca en la subsistencia inmediata, no en metas a futuro.',
          mensaje_incorrecto:
            '¡Continúe no se rinda! Equivocarse es aprender. Siga intentando, está en el camino correcto.',
        },
        {
          id: 7,
          texto:
            'El empoderamiento individual puede contribuir al desarrollo comunitario.',
          imagen: require('@/assets/actividad/imagen3.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'Verdadero', esCorrecta: true },
            { id: 'b', texto: 'Falso', esCorrecta: false },
          ],
          mensaje_correcto:
            'El empoderamiento individual impulsa la participación activa en proyectos colectivos.',
          mensaje_incorrecto:
            '¡Continúe no se rinda! Equivocarse es aprender. Siga intentando, está en el camino correcto.',
        },
        {
          id: 8,
          texto: 'El marco lógico no incluye la evaluación de riesgos.',
          imagen: require('@/assets/actividad/imagen4.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'Verdadero', esCorrecta: false },
            { id: 'b', texto: 'Falso', esCorrecta: true },
          ],
          mensaje_correcto:
            'El marco lógico considera riesgos y supuestos para mejorar la planificación.',
          mensaje_incorrecto:
            '¡Continúe no se rinda! Equivocarse es aprender. Siga intentando, está en el camino correcto.',
        },
        {
          id: 9,
          texto:
            'La formación ciudadana se basa solo en conocimientos técnicos.',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'Verdadero', esCorrecta: false },
            { id: 'b', texto: 'Falso', esCorrecta: true },
          ],
          mensaje_correcto:
            'Incluye competencias socioemocionales, cognitivas y comunicativas para la acción autónoma.',
          mensaje_incorrecto:
            '¡Continúe no se rinda! Equivocarse es aprender. Siga intentando, está en el camino correcto.',
        },
        {
          id: 10,
          texto:
            'El espacio privado es donde prevalece la dimensión individual.',
          imagen: require('@/assets/actividad/imagen2.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'Verdadero', esCorrecta: true },
            { id: 'b', texto: 'Falso', esCorrecta: false },
          ],
          mensaje_correcto:
            'En este ámbito, las personas fortalecen su identidad personal.',
          mensaje_incorrecto:
            '¡Continúe no se rinda! Equivocarse es aprender. Siga intentando, está en el camino correcto.',
        },
        {
          id: 11,
          texto:
            'La agencia proyectiva permite elaborar planes basados en recursos disponibles.',
          imagen: require('@/assets/actividad/imagen3.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'Verdadero', esCorrecta: true },
            { id: 'b', texto: 'Falso', esCorrecta: false },
          ],
          mensaje_correcto:
            'Este tipo de agencia se enfoca en metas a largo plazo.',
          mensaje_incorrecto:
            '¡No se preocupe por el error! Cada respuesta es una oportunidad para aprender y mejorar. Lo importante es seguir adelante y fortalecer los conocimientos.',
        },
        {
          id: 12,
          texto: 'El marco lógico es una herramienta exclusivamente académica.',
          imagen: require('@/assets/actividad/imagen4.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'Verdadero', esCorrecta: false },
            { id: 'b', texto: 'Falso', esCorrecta: true },
          ],
          mensaje_correcto:
            'Se utiliza en diversos contextos, desde organizaciones hasta comunidades.',
          mensaje_incorrecto:
            '¡No se preocupe por el error! Cada respuesta es una oportunidad para aprender y mejorar. Lo importante es seguir adelante y fortalecer los conocimientos. ',
        },
        {
          id: 13,
          texto:
            'La autoestima no influye en las competencias socioemocionales.',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'Verdadero', esCorrecta: true },
            { id: 'b', texto: 'Falso', esCorrecta: false },
          ],
          mensaje_correcto:
            'La autoestima es clave para el desarrollo de competencias socioemocionales.',
          mensaje_incorrecto:
            '¡No se preocupe por el error! Cada respuesta es una oportunidad para aprender y mejorar. Lo importante es seguir adelante y fortalecer los conocimientos. ',
        },
        {
          id: 14,
          texto:
            'El contexto social influye en las interacciones cotidianas y decisiones colectivas.',
          imagen: require('@/assets/actividad/imagen2.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'Verdadero', esCorrecta: true },
            { id: 'b', texto: 'Falso', esCorrecta: false },
          ],
          mensaje_correcto:
            'Este contexto define relaciones e impactos en la sociedad.',
          mensaje_incorrecto:
            '¡No se preocupe por el error! Cada respuesta es una oportunidad para aprender y mejorar. Lo importante es seguir adelante y fortalecer los conocimientos. ',
        },
        {
          id: 15,
          texto:
            'El marco lógico organiza los objetivos en una matriz clara y estructurada.',
          imagen: require('@/assets/actividad/imagen3.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'Verdadero', esCorrecta: true },
            { id: 'b', texto: 'Falso', esCorrecta: false },
          ],
          mensaje_correcto:
            'Su formato facilita la planificación y seguimiento del proyecto.',
          mensaje_incorrecto:
            '¡No se preocupe por el error! Cada respuesta es una oportunidad para aprender y mejorar. Lo importante es seguir adelante y fortalecer los conocimientos. ',
        },
        {
          id: 16,
          texto: 'La ciudadanía activa solo ocurre en espacios públicos.',
          imagen: require('@/assets/actividad/imagen4.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'Verdadero', esCorrecta: false },
            { id: 'b', texto: 'Falso', esCorrecta: true },
          ],
          mensaje_correcto:
            'También se ejerce en contextos sociales, educativos y laborales.',
          mensaje_incorrecto:
            '¡No se preocupe por el error! Cada respuesta es una oportunidad para aprender y mejorar. Lo importante es seguir adelante y fortalecer los conocimientos. ',
        },
        {
          id: 17,
          texto:
            'La resiliencia no es una competencia relevante en contextos sociales.',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'Verdadero', esCorrecta: false },
            { id: 'b', texto: 'Falso', esCorrecta: true },
          ],
          mensaje_correcto:
            'La resiliencia es crucial para superar desafíos sociales.',
          mensaje_incorrecto:
            '¡No se preocupe por el error! Cada respuesta es una oportunidad para aprender y mejorar. Lo importante es seguir adelante y fortalecer los conocimientos. ',
        },
        {
          id: 18,
          texto: 'El diagnóstico inicial es una fase del marco lógico.',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'Verdadero', esCorrecta: true },
            { id: 'b', texto: 'Falso', esCorrecta: false },
          ],
          mensaje_correcto:
            'Permite analizar necesidades y recursos antes de diseñar un proyecto.',
          mensaje_incorrecto:
            '¡No se preocupe por el error! Cada respuesta es una oportunidad para aprender y mejorar. Lo importante es seguir adelante y fortalecer los conocimientos. ',
        },
        {
          id: 19,
          texto:
            'El espacio privado fomenta interacciones colectivas sobre intereses generales.',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'Verdadero', esCorrecta: false },
            { id: 'b', texto: 'Falso', esCorrecta: true },
          ],
          mensaje_correcto:
            'Este espacio se enfoca en la dimensión personal y familiar.',
          mensaje_incorrecto:
            '¡No se preocupe por el error! Cada respuesta es una oportunidad para aprender y mejorar. Lo importante es seguir adelante y fortalecer los conocimientos. ',
        },
        {
          id: 20,
          texto:
            'El marco lógico facilita el monitoreo y evaluación de proyectos.',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'Verdadero', esCorrecta: true },
            { id: 'b', texto: 'Falso', esCorrecta: false },
          ],
          mensaje_correcto:
            'Sus indicadores ayudan a medir avances y ajustar estrategias.',
          mensaje_incorrecto:
            '¡Continua no te rindas! Equivocarse es aprender. Sigue intentando, estás en el camino correcto. ¡Tú puedes!',
        },
      ],
      mensaje_final_aprobado:
        '¡Excelente! Lo felicito, ha superado la actividad y demuestra sólidos conocimientos sobre el componente formativo.',
      mensaje_final_reprobado:
        'No ha superado la actividad. Le recomendamos volver a revisar el componente formativo e intentar nuevamente la actividad didáctica.',
    },
  }),
}
</script>
