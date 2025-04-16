<script lang="ts">
  let name = "Svelte";
  import Nested from "./Nested.svelte";
</script>

<h1>Hello {name.toUpperCase()}!</h1>

<style>
  h1 {
    color:aqua;
  }
</style>
<Nested />
