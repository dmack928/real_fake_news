<template>
  <section class="section">
    <div class="container">
      <div class="columns is-multiline">
        <div
          v-for="(article, index) in articles"
          :key="index"
          class="column is-one-quarter">
          <a
            :href="article.url"
            target="_blank">
            <div class="card">
              <div class="card-image">
                <figure class="image is-1by1">
                  <img
                    :src="article.urlToImage"
                    :alt="article.title">
                </figure>
              </div>
              <div class="card-content">
                <div class="content">{{ article.title }}</div>
              </div>
            </div>
          </a>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  async asyncData({ app }) {
    const { articles } = await app.$axios.$get(
      `https://newsapi.org/v2/top-headlines?sources=nhl-news&apiKey=fde33ade4c27470bb1f9062cbf6e9d42`
    )

    return { articles }
  }
}
</script>
