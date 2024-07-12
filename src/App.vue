<template>
  <ul>
    <ResourceItem 
      v-for="resource in storeResourses" 
      :title="resource.title" 
      :description="resource.description"
      :link="resource.link">
    </ResourceItem>
  </ul>
</template>

<script>
import ResourceItem from './components/ResourceItem.vue'

export default {
  data() {
    return {
      storeResourses: [
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
  components: {
    ResourceItem,
  }
}</script>