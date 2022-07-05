<template>
  <div>
    <b-container>
      <b-row>
        <b-col>
          <b-card
            title="Nemzeti Művelődési Intézet Nonprofit Közhasznú  Kft."
           >
            <b-card-text>
<h3>Kistelepülési önkormányzatok rendezvényeinek támogatása</h3>

<div v-for = "imgs in 6" :key="imgs" class="mt-3">

    <b-img fluid :src="'/nmi2021/'+imgs+'.jpg'"></b-img>
</div>
            </b-card-text>
          </b-card>
        </b-col>
      </b-row>
    </b-container>
  </div>
</template>