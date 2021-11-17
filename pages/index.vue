<template>
  <div>
    <b-container>
      <b-row>
        <b-col>
           <div>
  <b-img src="/gacsalyreftemp.jpg" fluid-grow alt="Gacsályi templom"></b-img>
</div>
          <div v-for="article of articles" :key="article.number">
            <b-card tag="article" style="max-width: 100%" class="mb-2">
              <b-card-text>
                <h2>{{ article.title }}</h2>
                <article>
                  <nuxt-content :document="article" />
                </article>
              </b-card-text>
            </b-card>
          </div>
        </b-col>
      </b-row>
    </b-container>
  </div>
</template>

<script>
export default {
  async asyncData({ $content, params }) {
    const articles = await $content("articles")
      .sortBy("number", "desc")
      .fetch();

    return {
      articles,
    };
  },
};
</script>

<style>
.nuxt-content h2 {
  font-weight: bold;
  font-size: 28px;
}
.nuxt-content h3 {
  font-weight: bold;
  font-size: 22px;
}
.nuxt-content p {
  margin-bottom: 20px;
}
.nuxt-content ul {
  list-style-type: none;
}
</style>