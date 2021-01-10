<template>
  <nav>
    <p class="caveat">
      {{ $t("header.builtby") }}
      <a href="https://twitter.com/mr_z_ro" target="_blank">mr_z_ro</a>
    </p>
  </nav>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>

nav {
  font-size: 40px;
  font-weight: 700;
  text-shadow: 0px 2px 5px #000;
  text-align: right;
}

svg {
  vertical-align: middle;
  margin-top: -3px;
}

.caveat {
  font-family: "Caveat", cursive;
  font-size: 20px;
  margin-top: -10px;
  margin-bottom: 0px;
  color: #ffd908;
  opacity: 0.9;
  font-weight: normal;
}

a,
a:visited,
a:active {
  color: #ffd908;
  text-decoration: none;
}
</style>