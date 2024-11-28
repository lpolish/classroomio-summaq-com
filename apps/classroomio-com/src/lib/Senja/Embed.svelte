<script lang="ts">
  import { embedSenjaWidget } from 'shared/src/senja';
  import { onMount } from 'svelte';

  export let id = '';

  onMount(() => {
    embedSenjaWidget(id);
  });
</script>

<style>
 .dark .senja-embed {
    background-color: #1a202c !important;
  }
</style>

<div class="senja-embed" data-id={id} data-lazyload="false" data-spinner="false"></div>
