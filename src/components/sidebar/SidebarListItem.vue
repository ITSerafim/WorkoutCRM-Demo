<template>
  <li class="list-style-none">
    <router-link
      :to="path ?? ''"
      class="txt-hover-primary trans-1 text-regular text-decor-none txt-color-addit-2 flex ai-center gap-25"
      active-class="link-active"
    >
      <font-awesome-icon :icon="icon" />{{ name }}</router-link
    >
  </li>
</template>

<script setup lang="ts">
import { Route } from '../../shared/types/Route';

defineProps<Route>();
</script>
