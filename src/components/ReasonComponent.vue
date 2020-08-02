<template>
  <v-layout row align-center justify-center style="background-color:;" >
      <v-col cols="12" md="9">
          <v-card class="mt-6" flat align="center" justify="center" style="background-color:;">
            <v-card-title primary-title class="layout justify-center mt-8"><h2>5 hyvää syytä valita Accountor Online taloushallintopalvelu</h2></v-card-title>
                <v-expansion-panels focusable flat class="mt-6">
                    <v-expansion-panel v-for="item in items" :key="item.id">
                    <v-expansion-panel-header class="font-weight-bold">{{ item.question }}</v-expansion-panel-header>
                    <v-expansion-panel-content>
                        <p class="caption text-left mt-4"> {{ item.info }} </p>
                    </v-expansion-panel-content>
                    </v-expansion-panel>
                </v-expansion-panels>
            </v-card>
      </v-col>
    </v-layout>
</template>

<script>
export default {
    data: () => {
      return {
          items: [
              {
                  id: '1',
                  question: "1. Saat samassa paketissa kaiken, mitä tarvitset yrityksesi taloushallintoon",
                  info: "Accountor Online tarjoaa ratkaisun, joka kattaa kaikki taloushallinnon osa-alueet mukaan lukien raportoinnin. Sinulla on pääsy helppokäyttöiseen ohjelmistoon, jossa voit tehdä haluamasi kirjaukset tai vain seurata ulkoistetun työn etenemistä. Palvelun käyttöönoton yhteydessä teemme tarvekartoituksen, jonka pohjalta sovimme työnjaosta sinun ja kirjanpitäjäsi välillä. Työnjako on sovittavissa joustavasti.",
              },
               {
                  id: '2',
                  question: "2. Saat avuksesi oman nimetyn kirjanpitäjän",
                  info: "Kun olet meillä asiakkaana, palvelusta vastaa sama asiantuntija kuukaudesta toiseen. Läheisen yhteistyön kautta asiantuntijamme oppivat tuntemaan asiakkaansa, heidän liiketoimintansa ja tarpeensa. Mahdollisista ongelmista ei tarvitse selvitä yksin, vaan asiantuntijamme opastavat ja neuvovat niin kirjanpidon kuin taloushallinnon kysymyksissä laajemminkin. Asiantuntijamme ovat aina käytettävissäsi – sähköpostitse, puhelimitse ja kasvokkain.",
              },
               {
                  id: '3',
                  question: "3. Saat nopeaa palvelua ja aina ajantasaiset tiedot",
                  info: "Accountor Online asiakkaana saat käyttöösi kirjanpidon Procountor -ohjelmiston. Pilvipalveluna toimiva ohjelmisto mahdollistaa, että kaikki yrityksesi taloustiedot ovat saatavillasi ajasta ja paikasta riippumatta, myös mobiilisti. Voit hakea raportit helposti ja nopeasti suoraan ohjelmistosta. Ajantasainen talouden seuraaminen ja ennustaminen on suuri etu yrityksen talouden ylläpitämisessä ja kehittämisessä.",
              },
               {
                  id: '4',
                  question: "4. Sujuvaa taloushallintoa mobiilisovelluksella",
                  info: "Procountorin älypuhelimeen ladattavalla, maksuttomalla Mini-sovelluksella voit tarkistaa ja hyväksyä laskut vaikka tien päällä ollessasi. Voit myös tehdä matkalaskun valmiiksi jo matkan aikana. Tämän lisäksi kuittien skannaaminen ja tallentaminen onnistuu helposti, jolloin paperisia versioita ei enää tarvitse säilyttää.",
              },
               {
                  id: '5',
                  question: "5. Hinnoittelu on selkeää ja läpinäkyvää",
                  info: "Maksat palvelusta ja järjestelmästä toteutuneiden tositemäärien mukaan – ei piilokuluja tai yllättäviä kustannuksia. Accountor Online on markkinoiden ainoa puhtaasti toteutuneeseen tositeveloitukseen perustuva taloushallinnon kokonaispalvelu. Jokaiselle tositelajille on sovittu kappalehinta, jonka perusteella laskutamme asiakasta vain toteutuneiden määrien mukaan. Tositekohtainen hinta sisältää kaikki kustannukset sekä tehdystä työstä että järjestelmästä. Asiakkaana voit lisäksi tarkistaa kuukausittaiset tositemäärät reaaliaikaisesti palvelusta. Pääkirjanpidolle puolestaan sovimme yhden kuukausihinnan, jonka laskutamme tasaisesti ympäri vuoden. Asiakkaanamme pystytkin ennustamaan yrityksesi taloushallinnon kulut entistä paremmin.",
              },
          ]
      }
      }
}
</script>

<style>

</style>