<script>
  import { link } from "svelte-routing";

  export let href;
  export let isCurrent = false;
</script>

<style>
  a:hover,
  a.current {
    background: #444;
    color: #f7c08a;
  }
  a {
    display: block;
    padding: 20px;
    text-align: center;
    color: #fff;
  }
</style>

<a class:current={isCurrent} use:link {href}>
  <slot />
</a>
