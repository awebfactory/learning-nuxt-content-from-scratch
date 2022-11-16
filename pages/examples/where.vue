<script lang="ts" setup>
const projects = await queryContent("projects").find()
console.log(projects)
</script>

<template>
  <main>
    <section>
      <ContentQuery
        path="/examples"
        find="one"
        :where="{ title: 'Query Where' }"
        v-slot="{ data }"
      >
        <ContentRenderer :value="data">
          <p>Mood: {{ data.mood }} See below for <em>Projects listing</em></p>
          <ContentRendererMarkdown :value="data" />
        </ContentRenderer>
      </ContentQuery>
    </section>
    <section>
      <h2 id="#projects">Projects</h2>
      <p>
        Find and list all projects in the
        <code>~/content/projects</code> directory
      </p>
      <code> const projects = await queryContent("projects").find() </code>
      <ul v-if="projects">
        <li v-for="project in projects" :key="project.slug">
          <NuxtLink :to="`/projects/${project.slug}`" className="mt-2 block">
            <p
              className="text-xl font-semibold text-orange-peel-800 hover:text-wild-willow-400"
            >
              {{ project.title }}
            </p>
            <p className="mt-3 text-base text-gray-500">
              {{ project.description }}
            </p>
          </NuxtLink>
        </li>
      </ul>
    </section>
  </main>
</template>

<style scoped></style>
