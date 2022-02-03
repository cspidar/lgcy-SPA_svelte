<script context="module" lang="ts">
    import { path } from 'svelte-pathfinder'

    import { appName } from '../lib/constants'
</script>

<script lang="ts">
    export let title = ''
</script>

<svelte:head>
    <title>{`${title ? title + ' | ' : ''}${appName}`}</title>
</svelte:head>

<main>
    <slot />
    <footer />
</main>
