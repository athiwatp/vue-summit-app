<template>
  <BasePage class="page-home">
    <h1>Sessions</h1>
    <SessionList
      :query="require('../graphql/SessionsPublic.gql')"
      data-prop="sessionsPublic"
    />
  </BasePage>
</template>

<script>
import SessionList from './SessionList.vue'

export default {
  components: {
    SessionList,
  },
}
</script>
