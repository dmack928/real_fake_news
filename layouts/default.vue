<template>
  <div>
    <section class="hero has-text-centered is-dark is-small">
      <div class="hero-body">
        <div class="container">
          <h1 class="title"> The Sports Cache</h1>
          <h2 class="subtitle">Up to the minute Sporting news!</h2>
        </div>
        <div>
          <ul>
            <nuxt-link to="/nfl"> NFL  </nuxt-link>
            <nuxt-link to="/nhl"> NHL  </nuxt-link>
          </ul>
        </div>
      </div>
      <nuxt-link to="/"> Home </nuxt-link>
    </section>
    <nuxt/>
  </div>
</template>
<style>
html {
  font-family: 'Source Sans Pro', -apple-system, BlinkMacSystemFont, 'Segoe UI',
    Roboto, 'Helvetica Neue', Arial, sans-serif;
  background: #ddffff;
}
</style>
