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
                <b-button variant="success" href="/doc/helyiado.pdf" download
                  >Letöltés</b-button
                >
                <b-button
                  variant="info"
                  href="/doc/helyiado.pdf"
                  target="blank"
                >
                  Megnyítás</b-button
                >
              </b-button-group>
              <br />
              {{ doc.desc }}
            </b-list-group-item>

            <b-list-group-item>
              <b-button-group class="mb-3">
                <b-button variant="success" href="/doc/helyiado.pdf" download
                  >Letöltés</b-button
                >
                <b-button
                  variant="info"
                  href="/doc/helyiado.pdf"
                  target="blank"
                >
                  Megnyítás</b-button
                >
              </b-button-group>
              <br />
              Gacsály Község Önkormányzata Képviselő-testületének 1/2018.(II.1.)
              önkormányzati rendelete a helyi adókról
            </b-list-group-item>

            <b-list-group-item>
              <b-button-group class="mb-3">
                <b-button
                  variant="success"
                  href="/doc/gacsaly-trt-szab-bt.pdf"
                  download
                  >Letöltés</b-button
                >
                <b-button
                  variant="info"
                  href="/doc/gacsaly-trt-szab-bt.pdf"
                  target="blank"
                >
                  Megnyítás</b-button
                >
              </b-button-group>
              <br />
              Belterületi szabályozási terv
            </b-list-group-item>

            <b-list-group-item>
              <b-button-group class="mb-3">
                <b-button
                  variant="success"
                  href="/doc/gacsaly-trt-szab-bt.pdf"
                  download
                  >Letöltés</b-button
                >
                <b-button
                  variant="info"
                  href="/doc/gacsaly-trt-szab-kt.pdf"
                  target="blank"
                >
                  Megnyítás</b-button
                >
              </b-button-group>
              <br />
              Külterületi szabályozási terv
            </b-list-group-item>

            <b-list-group-item>
              <b-button-group class="mb-3">
                <b-button
                  variant="success"
                  href="/doc/gacsaly-trt-szab-kt.pdf"
                  download
                  >Letöltés</b-button
                >
                <b-button
                  variant="info"
                  href="/doc/helyiado.pdf"
                  target="blank"
                >
                  Megnyítás</b-button
                >
              </b-button-group>
              <br />
              Településszerkezeti terv
            </b-list-group-item>

            <b-list-group-item>
              <b-button-group class="mb-3">
                <b-button
                  variant="success"
                  href="/doc/gacsaly-trt-szab-szerkterv.pdf"
                  download
                  >Letöltés</b-button
                >
                <b-button
                  variant="info"
                  href="/doc/helyiado.pdf"
                  target="blank"
                >
                  Megnyítás</b-button
                >
              </b-button-group>
              <br />
              Szabályozási terv és helyi építési szabályzat
            </b-list-group-item>

            <b-list-group-item>
              <b-button-group class="mb-3">
                <b-button
                  variant="success"
                  href="/doc/leiras_gacsaly_egyseges.pdf"
                  download
                  >Letöltés</b-button
                >
                <b-button
                  variant="info"
                  href="/doc/leiras_gacsaly_egyseges.pdf"
                  target="blank"
                >
                  Megnyítás</b-button
                >
              </b-button-group>
              <br />
              Településszerkezeti terv és leírása
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
        { desc: "sdads", sa: "ssss" },
        { desc: "sdads", link: "ssss" },
        { desc: "sdads", link: "ssss" },
        { desc: "sdads", link: "ssss" },
        { desc: "sdads", link: "ssss" },
        { desc: "sdads", link: "ssss" },
      ],
    };
  },
};
</script>
