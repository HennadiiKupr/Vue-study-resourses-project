<template>
  <li>
    <h1>{{ title }}</h1>
    <a :href="link">
      <p>{{ description }}</p>
    </a>
  </li>
</template>

<script>
export default {
  props: ['title', 'description', 'link']
}
</script>