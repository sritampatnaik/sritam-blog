<template>
  <Layout>
    <header class="header">
      <h1 v-html="$page.metadata.siteName" />
      <h2 v-html="$page.metadata.siteDescription" />
    </header>
    <section class="main-body">
      <g-link to="/blog" class="btn"> Blog &rarr;</g-link>
    </section>

  </Layout>
</template>

<script>
export default {
  metaInfo: {
    title: "A simple blog",
  },
};
</script>

<page-query>
query {
  metadata {
    siteName
    siteDescription
  }
}
</page-query>

<style>
.header {
  font-family: "Inconsolata";
  font-size: 35px;
  text-align: center;
  line-height: 1.6em;
  padding: 0.7em;
}

.header h2 {
  font-weight: 200;
  font-size: 35px;
}

.main-body {
  text-align: center;
}

</style>
