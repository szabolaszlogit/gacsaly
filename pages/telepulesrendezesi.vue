<template>
  <div>
    <b-container>
      <b-row>
        <b-col>
          <b-jumbotron
            header="Településrendezési terv"
            lead="Letölthető anyagok és dokumentumok"
          >
          </b-jumbotron>
          <b-list-group v-for="doc in docs" :key="doc.desc">
            <b-list-group-item>
              <b-button-group class="mb-3">
                <b-button
                  variant="success"
                  :href="'/telepulesrendezesi/' + doc.link"
                  download
                  >Letöltés</b-button
                >
                <b-button
                  variant="info"
                  :href="'/telepulesrendezesi/' + doc.link"
                  target="blank"
                >
                  Megnyítás</b-button
                >
              </b-button-group>
              <br />
              {{ doc.desc }}
            </b-list-group-item>
          </b-list-group>
        </b-col>
      </b-row>
    </b-container>
  </div>
</template>

<script>
export default {
  data() {
    return {
      docs: [
        {
          desc: "Gacsály RT módosítás - 2022 I. - ETD - Főeljárás",
          link: "gacsaly_rt_modositas_2022_1_etd_foeljaras.pdf",
        },
        {
          desc: "Gacsály RT módosítás - 2022 I. - ETD - Környezeti vizsgálat",
          link: "gacsaly_rt_modositas_2022_1_etd_kornyezeti.pdf",
        },
        {
          desc: "Gacsály RT módosítás - 2022 I. - ETD - Térségi övezeti",
          link: "gacsaly_rt_modositas_2022_1_etd_tersegi.pdf",
        },
        {
          desc: "Gacsály RT módosítás - 2022 I. - Véleményezési dokumentáció",
          link: "gacsaly_rt_modositas_2022_1_velemenyezesi_dokumentacio.pdf",
        },
      ],
    };
  },
};
</script>
