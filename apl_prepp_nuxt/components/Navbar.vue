<template>
  <div class="nav">
    <a href="/">Home</a>
    <a href="/dashboard">Dashboard</a>
    <a href="/welcome">Welcome page</a>
  </div>
</template>

<script>
export default {
  name: 'Navbar'
}
</script>

<style scoped>
.nav {
  display: flex;
  justify-content: center;
  align-items: center;
}

a {
  font-size: 2rem;
  padding: 0rem 1rem;
}

a:hover {
  text-decoration: underline;
  background: lightgrey;
}

a:active {
  background: grey;
}
</style>
