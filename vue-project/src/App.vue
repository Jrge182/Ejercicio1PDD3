<template>
  <div id="app">
    <h1>Presentacion de VUE</h1>

    <div v-if="ver">
      <p>Vue.js es un framework de JavaScript de código abierto para 
      la construcción de interfaces de usuario y aplicaciones de una sola página. 
      Fue creado por Evan You, y es mantenido por él y por el resto 
      de los miembros activos del equipo central que provienen de diversas 
      empresas como Netlify y Netguru</p>
      
      <li>
      La curva de aprendizaje es, con diferencia, la más 
      sencilla de los tres frameworks más populares: React, Vue y Angular.
      </li>

      <p></p>
      <li>
      Se trata de un framework muy amigable y respetuoso con 
      las tecnologías de frontend y los estándares. 
      Utiliza HTML, CSS y Javascript y es compatible con WebComponents 
      (de hecho, sus componentes se basan en ellos). Si eres desarrollador 
      con base fuerte de HTML/CSS, muy probablemente te guste más Vue que otras opciones.
      </li>
      
      <p></p>
      <li>
      Se trata de un framework progresivo. Esto significa que es 
      ideal para migrar y adaptar proyectos existentes hechos en otras tecnologías
       y pasarlos poco a poco a Vue. Algo muy común cuando trabajas en proyectos legacy 
       (la mayoría de los casos en muchas empresas).
      </li>

      <p></p>
      <li>
      Los desarrolladores que provienen de lenguajes o frameworks exclusivamente 
      de backend están acostumbrados a ciertos patrones de programación que no son 
      exactamente iguales en frontend. Es aconsejable aprender ciertas bases 
      de frontend general. Una buena base de Javascript también es muy recomendable.
      </li>

      <p></p>
      <li>
      Vue le da mayor protagonismo al enfoque tradicional «centrado en HTML», 
      así como a los sistemas de plantillas. Si te gustan, 
      Vue probablemente te resulte muy atractivo. Por otro lado, el enfoque de React 
      se suele centrar más en programación pura en Javascript, utilizando 
      HTML y CSS sólo como complementos que se añaden a Javascript.
      </li>
    </div>


    <button @click="mostrar">Mostrar</button>
    <button @click="ocultar">Ocultar</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      ver: false,
    };
  },

  methods: {
    mostrar() {
      this.ver = true;

    },

    ocultar() {
      this.ver = false;
    }
  }
};
</script>