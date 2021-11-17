<template>
  <div>
    <b-container>
      <b-row>
        <b-col>
          <b-card
            title="VP6-7.2.1-7.4.1.2-16"
            img-src="/infoblokk_emva.jpg"
            img-alt="Gacsály Művelődési ház"
            img-top
            tag="article"
            style="max-width: 100%"
            class="mb-2"
          >
            <b-card-text>
              Kedvezményezett neve: <br />
              Gacsály Község Önkormányzata <br />
              Pályázati felhívás neve, kódszáma: <br />
              Külterületi helyi közutak fejlesztése és önkormányzati utak
              kezelését biztosító gépek beszerzése -VP6-7.2.1-7.4.1.2-16 <br />
              Projekt címe, azonosító száma: <br />
              Gacsály 0136 hrsz-ú önkormányzati tulajdonú külterületi helyi
              közút fejlesztése - 1826746675 <br />
              Szerződött támogatás összege: 96.016.855,-Ft <br />
              Támogatás mértéke (%-ban): 95,00 % <br />
              Projekt tartalmának rövid bemutatása: <br />
              A beavatkozás célja a Gacsályt Túrricsével összekötő TELEPÜLÉSKÖZI
              ÚT - 2003 évben szilárd burkolattal ellátott szakaszának
              folytatásaként - a meglévő 0136 hrsz-ú földút alépítményének és
              burkolatának kialakítása, vízelvezetés kialakítása. lásd csatolt
              A-1 Átnézeti helyszínrajzon is. A tervezési szakasz 1566 m hosszú.
              A tervezett útszakasz önkormányzati utakhoz csatlakozik. A projekt
              tárgyát képező 0136 helyrajzi számú külterületi közút Gacsályt
              Túrricsével összekötő TELEPÜLÉSKÖZI ÚT. <br />
              Gacsály irányából 2003 évben szilárd burkolattal ellátott első
              szakaszának folytatásaként a meglévő földút alépítményének és
              burkolatának, valamint a vízelvezetés kialakításának realizálása
              jelenprojekt tárgya. Ezáltal a két település - továbbá a környező
              települések - közötti gazdasági és egyéb lakossági
              gépjárműforgalom válik könnyebbé. Hangsúlyos szempont, hogy a
              2003. évben megvalósult szilárd burkolattal ellátott első szakasz
              beruházása is a folytatással válik még inkább hasznossá, azaz a
              két projekt egymást felerősítő hatást vált ki, mind az
              indokoltság, mind a befektetett pénztőke gazdasági és társadalmi
              megtérülését tekintve. Korábban nagyobb esőzések után, tavaszi
              olvadáskor a kátyúk, a felázások teljesen lehetetlenné tették a
              közlekedést a még ki nem épült úton. Abban az időszakban
              személyautó forgalomra az útszakasz teljesen alkalmatlan volt.
              Mára az előbb említett problémák megoldódtak, így a településen és
              környéken élők régi vágya valósult meg. Projekt tervezett
              befejezési dátuma: 2020.06.30. <br />

              <br />
              „Gacsály 0136 hrsz-ú önkormányzati tulajdonú külterületi helyi
              közút fejlesztése” című VP6-7.2.1-7.4.1.2-16 kódszámú 1826746675
              azonosító számú projekt <br />

              <b-list-group v-for="doc in docs" :key="doc.desc">
                <b-list-group-item>
                  <b-button-group class="mb-3">
                    <b-button
                      variant="success"
                      :href="'/doc/' + doc.link"
                      download
                      >Letöltés</b-button
                    >
                  </b-button-group>
                  <br />
                  {{ doc.desc }}
                </b-list-group-item>
              </b-list-group>
            </b-card-text>
          </b-card>
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
          desc: "Összegezést az ajánlatok elbírálásáról",
          link: "xmldata2.pdf",
        },
        {
          desc: "Benyújtott ajánlatok jegyzőkönyve (Bontási jegyzőkönyv)",
          link: "xmldata.pdf",
        },
        {
          desc: "Ajánlattételi felhívás módosítása és ajánlattételi határidő meghosszabbítása",
          link: "ajanlattetel_modositas.pdf",
        },
        {
          desc: "A teljesítésbe bevonásra kerülő műszaki szakember szakmai önéletrajza",
          link: "oneletrajz.doc",
        },
        {
          desc: "Ajánlattételi felhívás",
          link: "ajanlatteteli-felhivas.pdf",
        },
        {
          desc: "Dokumentáció és szerződés-tervezet",
          link: "dokumentacio-es-szerzodes-tervezet.pdf",
        },
        {
          desc: "DKiviteli tervek,műszaki leírás, építési engedély",
          link: "kiviteli-tervek-muszaki-leiras-epitesi-engedely.zip",
        },
        {
          desc: "Költségvetés árazatlan Gacsály 2018.12.19.",
          link: "koltsegvetesi-arazattan-gacsaly-20181219.xls",
        },
        {
          desc: "Nyilatkozat kizáró okokról",
          link: "nyilatkozat-kizaro-okrol.doc",
        },
      ],
    };
  },
};
</script>