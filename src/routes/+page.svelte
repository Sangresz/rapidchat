<script lang="ts">
    import type { Country } from "$lib/types";

    export let data: {countries: Country[]}
</script>

<h1>Welcome to SvelteKit</h1>
<p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>

{#each data.countries as country}
    <li>
        {country.name}
    </li>
{/each}