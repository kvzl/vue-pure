<template>
  <nav id="nav">
    <ul>
      <router-link tag="li" to="/">
        <a>Counter</a>
      </router-link>
      <router-link tag="li" to="/board">
        <a>Board</a>
      </router-link>
    </ul>
  </nav>
</template>

<script>
export default {
  name: 'Navigation',
}
</script>

<style scoped lang="scss">

#nav {
  height: 60px;
  width: 100%;
  box-shadow: 0px 2px 5px 0px #cacaca;
  text-align: left;
}

ul {
  height: 100%;
  display: flex;
  align-items: center;
  list-style: none;
  margin-block-start: 0;
  margin-block-end: 0;
}

li {
  margin-right: 20px;

  &.router-link-exact-active a {
    color: black;
  }
}

a {
  text-decoration: none;
  color: darkcyan;
}

</style>
