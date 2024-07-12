<template>
  <StoredResources :resources="storedResourses" />
</template>

<script>
import StoredResources from './components//learning-resources/StoreResources.vue'
import LearningResource from './components/learning-resources/LearningResource.vue';

export default {
  components: {
    LearningResource,
    StoredResources
  },
  data() {
    return {
      storedResourses: [
        {
          id: 'official-guide',
          title: 'Official Guide',
          description: 'The official Vue.js documentation',
          link: 'https://vuejs.org'
        },
        {
          id: 'google',
          title: 'Google',
          description: 'Learn to google...',
          link: 'https://google.com'
        },
      ]
    }
  },
};
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap');

* {
  box-sizing: border-box;
}

html {
  font-family: 'Roboto', sans-serif;
}

body {
  margin: 0;
}
</style>