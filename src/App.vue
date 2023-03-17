<template>
  <section>
    <div>
      <h1>Hello my name is Rodion Voinarovskyi.</h1>
      <h2>And here you can see my works</h2>
    </div>
    <ul>
      <li v-for="item in portfolioItems" :key="item.id">
        <a :href="item.url" target="_blank">{{ item.title }}</a>
      </li>
    </ul>
  </section>
</template>

<script>
export default {
  data() {
    return {
      portfolioItems: [
        {
          title: "Weather App",
          url: "https://weather-app-43602.web.app/",
        },
        {
          title: "To Do App",
          url: "https://vue-todo-362bb.web.app/",
        },
        {
          title: "Meals Library App",
          url: "https://meal-library.web.app/",
        },
        {
          title: "Adventure Notes App",
          url: "https://adventure-notes.web.app/",
        },
      ],
    };
  },
};
</script>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
