<template>
  <div>
    <b-container>
      <b-row>
        <b-col>
          <b-jumbotron
            header="Dokumentumok"
            lead="Letölthető anyagok és dokumentumok"
          >
          </b-jumbotron>
          <b-list-group v-for="doc in docs" :key="doc.desc">
            <b-list-group-item>
              <b-button-group class="mb-3">
                <b-button variant="success" :href="'/doc/' + doc.link" download
                  >Letöltés</b-button
                >
                <b-button
                  variant="info"
                  :href="'/doc/' + doc.link"
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
          desc: "Gacsály Község Önkormányzata Képviselő-testületének 1/2018.(II.1.) önkormányzati rendelete a helyi adókról",
          link: "helyiado.pdf",
        },
        {
          desc: "Belterületi szabályozási terv",
          link: "gacsaly-trt-szab-bt.pdf",
        },
        {
          desc: "Külterületi szabályozási terv",
          link: "gacsaly-trt-szab-kt.pdf",
        },
        {
          desc: "Településszerkezeti terv",
          link: "gacsaly-trt-szab-szerkterv.pdf",
        },
        {
          desc: "Szabályozási terv és helyi építési szabályzat",
          link: "hesz_gacsaly_egyseges.pdf",
        },
        {
          desc: "Településszerkezeti terv és leírása",
          link: "leiras_gacsaly_egyseges.pdf",
        },
      ],
    };
  },
};
</script>
