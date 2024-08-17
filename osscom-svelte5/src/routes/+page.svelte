<h1>Welcome to SvelteKit</h1>
<p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>
<script>
    let count = $state(0);
</script>

<button on:click={() => count++}>
    clicks: {count}
</button>