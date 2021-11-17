<template>
  <nav>
    <b-container-fluid>
      <b-row>
        <b-col>
          <div>
            <b-navbar toggleable="lg" type="light" variant="success">
              <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

              <b-collapse id="nav-collapse" is-nav>
                <b-navbar-nav>
                  <b-nav-item>
                    <NuxtLink to="/">Gacsály</NuxtLink>
                  </b-nav-item>

                  <b-nav-item-dropdown text="Településünk" right>
                    <div class="bg-secondary">
                      <b-dropdown-item>
                        <NuxtLink to="/about">Gacsályról</NuxtLink>
                      </b-dropdown-item>
                      <b-dropdown-item>
                        <NuxtLink to="/latnivalok"> Látnivalók</NuxtLink>
                      </b-dropdown-item>
                    </div>
                  </b-nav-item-dropdown>

                  <b-nav-item>
                    <NuxtLink to="/doc">Dokumentumok</NuxtLink></b-nav-item
                  >
                  <b-nav-item>
                    <NuxtLink to="/helyiado">Helyi adó</NuxtLink></b-nav-item
                  >
                  <b-nav-item>
                    <NuxtLink to="/oktatas">Oktatás</NuxtLink></b-nav-item
                  >

                  <b-nav-item>
                    <NuxtLink to="/intezmenyek"
                      >Intézmények, vállakozók</NuxtLink
                    ></b-nav-item
                  >

                  <b-nav-item>
                    <NuxtLink to="/hivatal">Polgármesteri Hivatal</NuxtLink>
                  </b-nav-item>

                  <b-nav-item-dropdown
                    text="Egészségügy, szociális ügyek"
                    right
                  >
                    <div class="bg-secondary">
                      <b-dropdown-item>
                        <NuxtLink to="/haziorvos"> Háziorvos </NuxtLink>
                      </b-dropdown-item>
                      <b-dropdown-item>
                        <NuxtLink to="/vedono"> Védőnő </NuxtLink>
                      </b-dropdown-item>
                      <b-dropdown-item>
                        <NuxtLink to="/gyogyszertar"> Gyógyszertár </NuxtLink>
                      </b-dropdown-item>
                      <b-dropdown-item>
                        <NuxtLink to="/maltai">
                          Máltai Szeretetszolgálat
                        </NuxtLink>
                      </b-dropdown-item>
                      <b-dropdown-item>
                        <NuxtLink to="/idosek"> Idősek klubja </NuxtLink>
                      </b-dropdown-item>
                      <b-dropdown-item>
                        <NuxtLink to="/gyermekjolet"> Gyermekjólét </NuxtLink>
                      </b-dropdown-item>
                      <b-dropdown-item>
                        <NuxtLink to="/allatorvos"> Állatorvos </NuxtLink>
                      </b-dropdown-item>
                    </div>
                  </b-nav-item-dropdown>

                  <b-nav-item-dropdown text="Pályázatok" right>
                    <div class="bg-secondary">
                      <b-dropdown-item>
                        <NuxtLink to="/vp6721741216">
                          VP6-7.2.1-7.4.1.2-16
                        </NuxtLink>
                      </b-dropdown-item>
                      <b-dropdown-item>
                        <NuxtLink to="/mfpotu2019"> MFP-ÖTU/2019 </NuxtLink>
                      </b-dropdown-item>
                    </div>
                  </b-nav-item-dropdown>
                </b-navbar-nav>
              </b-collapse>
            </b-navbar>
          </div>
        </b-col>
      </b-row>
    </b-container-fluid>
  </nav>
</template>

<style>
.nuxt-link-active {
  color:lightyellow
}
a{
  color:black
}
</style>