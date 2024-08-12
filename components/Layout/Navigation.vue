<script>
import { ROUTES } from "~/constants/routes";

export default {
  name: "Navigation",
  computed: {
    ROUTES() {
      return ROUTES;
    },
  },
};
</script>

<template>
  <nav>
    <ul>
      <li>
        <nuxt-link :to="ROUTES.HOME">Home</nuxt-link>
      </li>
      <li>
        <nuxt-link :to="ROUTES.POSTS">Posts</nuxt-link>
      </li>
      <li>
        <nuxt-link :to="ROUTES.LOGIN">Login</nuxt-link>
      </li>
      <li>
        <nuxt-link :to="ROUTES.REGISTER">Register</nuxt-link>
      </li>
    </ul>
  </nav>
</template>

<style scoped></style>
