<script context="module" lang="ts">
    import Layout from '../components/Layout.svelte'
    import LinkButton from '../components/LinkButton.svelte'
    import { appName } from '../lib/constants'
</script>

<Layout>
    <div>
        <h1>
            {appName}
        </h1>
    </div>
</Layout>
