<template>
  <div>
    <h1>{{ title }}</h1>
    <p>{{ content }}</p>
    <button @click="addPost" type="button" class="btn btn-secondary">
      Click
    </button>
    <ul>
      <h3></h3>
      <p></p>
    </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {
      title: "",
      content: "",
      posts: []
    };
  },
  methods: {
    addPost() {
      fetch(
        "https://gnews.io/api/v4/top-headlines?token=dddc5a8bc6634be876db4d293248c833&lang=en"
      )
        .then((res) => {
          if (res.ok) {
            return res.json();
          }
        })
        .then((data) => {
          const posts = [];
          posts.push(data)
          this.posts=posts
        });
    },
  },
};
</script>
