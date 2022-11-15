---
mood: 👴
---

# Query Where

- Displaying this markdown partial inside a regularly created and routed Nuxt 3 vue page using the [ContentQuery](https://content.nuxtjs.org/api/components/content-query) component:

```vue
<template>
  <ContentQuery
    path="/examples"
    find="one"
    :where="{ title: 'Query Where' }"
    v-slot="{ data }"
  >
    <!--
    <pre>
      {{ data }}
    </pre>
    -->
    <ContentRenderer :value="data">
      <p>Mood: {{ data.mood }}</p>
      <ContentRendererMarkdown :value="data" />
    </ContentRenderer>
</template>
```
