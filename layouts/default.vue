<template>
  <div>
    <section class="hero has-text-centered is-dark">
      <div class="hero-body">
        <div class="container">
          <h1 class="title"> Sports Hook</h1>
          <h2 class="subtitle">Up to the minute Sporting news!</h2>
        </div>
        <div>
          <nuxt-link to="/"> Home </nuxt-link>
        </div>
        <div>
          <nuxt-link to="/nfl"> NFL News </nuxt-link>
        </div>
        <div>
          <nuxt-link to="/nhl"> NHL News </nuxt-link>
        </div>
      </div>
    </section>
    <nuxt/>
  </div>
</template>

<style>
html {
  font-family: 'Source Sans Pro', -apple-system, BlinkMacSystemFont, 'Segoe UI',
    Roboto, 'Helvetica Neue', Arial, sans-serif;
}
</style>
