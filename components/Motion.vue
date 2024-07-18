<script setup>
const props = defineProps({
  cas: { type: Boolean, default: false }
})
</script>

<template>
  <div class="motion rounded-md my-4">
    <div v-if="cas">
      <div class="motion-to">
        <span class="label">A:</span>
        <span>
          <strong>MINISTERIO DE TRANSPORTES Y MOVILIDAD SOSTENIBLE</strong>

          Dirección General de Aviación Civil
        </span>
      </div>
      
      <div class="motion-scroll">
        <p><strong>ALEGACIONES</strong> al Plan de Acción asociado al Mapa Estratégico de Ruido (Fase IV) del Aeropuerto de València que ha sido publicado el miércoles 12 de junio de 2024 en el BOE, seco. V-B, pág. 32566, </p>

        <ol>
          <li>Establecer como prioridad la implementación inmediata del sistema de monitorización de ruidos y trayectorias en el aeropuerto.</li>
          <li>Realizar estudios dirigidos a establecer RESTRICCIONES EN LOS VUELOS NOCTURNOS comerciales para minimizarlos y no incorporar de nueces. Planificar el cierre del Aeropuerto entre las 23.00 horas y las 7.00 horas.</li>
          <li>Realizar encuestas de percepción subjetiva del ruido en las zonas habitadas próximas al aeropuerto, a fin de completar los datos de que se dispone. </li>
          <li>Realizar ESTUDIOS EPIDEMIOLÓGICOS en la población afectada.</li>
          <li>Realizar MEDICIONES IN SITU EN LAS VIVIENDAS AFECTADAS, tanto dentro de como fuera de la huella.</li>
          <li>Realizar MEDICIONES IN SITU en otros inmuebles afectados con usos diferentes al residencial pero no menos importantes, como por ejemplo equipaciones educativas, deportivos, industriales o terciarios, tanto dentro de como fuera de la huella.</li>
          <li>Ampliar, en su momento las INSONORIZACIONES a viviendas que, si bien no están dentro de la huella, sí que están muy próximas y que quedan desprotegidas. Es necesario que estas viviendas tengan, al menos, una protección que permita que los niveles de ruido sufridos sean similares a las viviendas que se encuentran dentro de la huella.</li>
          <li>Para las pruebas de motores que se realizan al aire libre, se propone la habilitación de la plataforma equipada con tres menajes de barreras acústicas. También la instalación de pantallas acústicas para mitigar la propagación de ruido.</li>
          <li>Verificar el cumplimiento de la Ley 7/2002, de 3 de diciembre, de protección contra la contaminación acústica. Aplicable en la Comunidad Valenciana, territorio donde está situado el aeropuerto de València.</li>
          <li>En materia urbanística, no aumentar las servidumbres acústicas ni inferir en las competencias propias de los municipios. Establecer los mecanismos compensatorios adecuados para paliar las externalidades negativas que causa la presencia del aeropuerto y su huella acústica.</li>
          <li>Promover la derogación de la disposición adicional segunda del Real Decreto 2591/1998, de 4 de diciembre, sobre la Ordenación de los Aeropuertos de Interés General y su Zona de Servicio, en ejecución del que se dispone en el artículo 166 de la Ley 13/1996, de 30 de diciembre, de Medidas Fiscales, Administrativas y de la Orden Social, de forma que no quedo el planeamiento sujeto a la voluntad del Aeropuerto ni de la Dirección General de Aviación Civil.</li>
          <li>Agilizar la tramitación, reduciendo los tiempos de las actuaciones en las viviendas afectadas por la huella acústica, las últimas tardaron casi 4 años.</li>
          <li>Que para garantizar tanto la salud pública como el bienestar de las personas más sensibles (niños y niñas, personas mayores y personas enfermas), las líneas de vuelo no tienen que atravesar las edificaciones sensibles, como por ejemplo residencias de personas mayores, colegios, escuelas infantiles y hospitales/centres de salud.</li>
          <li>Estudiar las ayudas para climatitzar las viviendas afectadas, puesto que durante el periodo estival aumentan los vuelos por motivos turísticos y el cierre de ventanas perjudica la calidad de vida de los vecinos.</li>
        </ol>
      </div>
    </div>
    <div v-else>
      <div class="motion-to">
        <span class="label">A:</span>
        <span>
          <strong>MINISTERI DE TRANSPORTS I MOBILITAT SOSTENIBLE</strong>

          Direcció General d’Aviació Civil
        </span>
      </div>
      
      <div class="motion-scroll">
        <p><strong>AL·LEGACIONS</strong> al Pla d’Acció associat al Mapa Estratègic de Soroll (Fase IV) de l’Aeroport de València que ha sigut publicat el dimecres 12 de juny de 2024 en el BOE, sec. V-B, pàg. 32566,</p>

        <ol>
          <li>Establir com a prioritat la implementació immediata del sistema de monitoratge de sorolls i trajectòries en l’aeroport. </li>
          <li>Realitzar estudis dirigits a establir RESTRICCIONS ALS VOLS NOCTURNS comercials per a minimitzar-los i no incorporar-ne de nous. Planificar el tancament de l’Aeroport entre les 23.00 hores i les 7.00 hores.</li>
          <li>Realitzar enquestes de percepció subjectiva del soroll en les zones habitades pròximes a l’aeroport, a fi de completar les dades de què es disposa.</li>
          <li>Realitzar ESTUDIS EPIDEMIOLÒGICS en la població afectada.</li>
          <li>Realitzar MESURAMENTS IN SITU EN LES VIVENDES AFECTADES, tant dins com fora de la petjada.</li>
          <li>Realitzar MESURAMENTS IN SITU en altres immobles afectats amb usos diferents al residencial però no menys importants, com ara equipaments educatius, esportius, industrials o terciaris, tant dins com fora de la petjada.</li>
          <li>Ampliar, en el seu moment les INSONORITZACIONS a vivendes que, si bé no estan dins de la petjada, sí que hi estan molt pròximes i que queden desprotegides. És necessari que estes vivendes tinguen, almenys, una protecció que permeta que els nivells de soroll patits siguen similars a les vivendes que es troben dins de la petjada.</li>
          <li>Per a les proves de motors que es realitzen a l’aire lliure, es proposa l’habilitació de la plataforma equipada amb tres paraments de barreres acústiques. També la instal·lació de pantalles acústiques per a mitigar la propagació de soroll.</li>
          <li>Verificar el compliment de la Llei 7/2002, de 3 de desembre, de protecció contra la contaminació acústica. Aplicable a la Comunitat Valenciana, territori on està situat l’aeroport de València.</li>
          <li>En matèria urbanística, no augmentar les servituds acústiques ni inferir en les competències pròpies dels municipis. Establir els mecanismes compensatoris adequats per a pal·liar les externalitats negatives que causa la presència de l’aeroport i la seua petjada acústica.</li>
          <li>Promoure la derogació de la disposició addicional segona del Reial decret 2591/1998, de 4 de desembre, sobre l’Ordenació dels Aeroports d’Interés General i la seua Zona de Servici, en execució del que es disposa en l’article 166 de la Llei 13/1996, de 30 de desembre, de Mesures Fiscals, Administratives i de l’Ordre Social, de manera que no quede el planejament subjecte a la voluntat de l’Aeroport ni de la Direcció General d’Aviació Civil.</li>
          <li>Agilitzar la tramitació, reduint els temps de les actuacions en les vivendes afectades per la petjada acústica, les últimes van tardar quasi 4 anys.</li>
          <li>Que per tal de garantir tant la salut pública com el benestar de les persones més sensibles (xiquets i xiquetes, persones majors i persones malaltes), les línies de vol no han de travessar les edificacions sensibles, com ara residències de persones majors, col·legis, escoles infantils i hospitals/centres de salut.</li>
          <li>Estudiar les ajudes per a climatitzar les vivendes afectades, ja que durant el període estival augmenten els vols per motius turístics i el tancament de finestres perjudica la qualitat de vida dels veïns.</li>
        </ol>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.motion {
  border: 1px var(--gray-300) solid;
  overflow: clip;
  color: var(--gray-900);

  &-to {
    display: flex;
    border-bottom: 1px var(--gray-300) solid;

    span {
      padding: 1rem;
    }

    .label {
      border-right: 1px var(--gray-300) solid;
    }

    strong {
      display: block;
    }
  }

  &-scroll {
    overflow: auto;
    height: 300px;
    padding: 1rem;
  }

  ol {
    list-style: lower-alpha;

    li {
      margin-bottom: 1rem;
    }
  }
}
</style>