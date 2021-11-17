<template>
  <div>
    <b-container>
      <b-row>
        <b-col>
          <b-card
            
            tag="article"
            style="max-width: 100%"
            class="mb-2"
          >
            <b-card-text>
              <article>
                <nuxt-content :document="article" />
              </article>
            </b-card-text>
          </b-card>
        </b-col>
      </b-row>
    </b-container>
  </div>
</template>



<script>
export default {
  async asyncData({ $content, params }) {
    const article = await $content("articles", params.slug).fetch();

    return { article };
  },
};
</script>