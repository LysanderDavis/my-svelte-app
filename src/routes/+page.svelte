<script lang="ts">
  import Nested from "./Nested.svelte";
  let count = $state(0);

  function increment() {
    count += 1;
  }
</script>

<button onclick={increment}>
  Clicked {count}
  {count === 1 ? "time" : "times"}
</button>

<Nested />
