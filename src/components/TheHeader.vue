<template>
  <section>
    <nav class="navbar navbar-default">
      <div class="container">
        <div class="navbar-header">
          <a class="navbar-brand" href="/">{{ title }}</a>
        </div>
        <ul class="nav navbar-nav navbar-right">
          <li id="home">
            <a href="/"> {{ home }} </a>
          </li>
          <li id="about"><a href="/about">ABOUT US</a></li>
          <li id="contact"><a href="/contact">CONTACT US</a></li>
        </ul>
      </div>
    </nav>
  </section>
</template>

<script>
export default {
  data() {
    return {
      title: "DAILY NEWS",
      home: "HOME",
    };
  },
};
</script>

<style scoped>
.navbar {
  padding-top: 15px;
  padding-bottom: 15px;
  border: 0;
  border-radius: 0;
  margin-bottom: 0;
  font-size: 12px;
  letter-spacing: 5px;
}
.navbar-nav li a:hover {
  color: #1abc9c !important;
}
</style>
