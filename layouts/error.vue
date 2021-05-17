<template>
  <div>
    <h1 v-if="error.statusCode === 404">Deso la page n'existe pas</h1>
    <h1 v-else>BUG BUG BUG</h1>
    <NuxtLink to="/">Page d'accueil</NuxtLink>
  </div>
</template>

<script>
  export default {
    props: ['error'],
    layout: 'error' // nous pouvons definir un layout personnalisé pour la page erreur
  }
</script>