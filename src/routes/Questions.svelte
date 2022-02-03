<script context="module" lang="ts">
    import Layout from '../components/Layout.svelte'
    import RandomQuestion from '../components/RandomQuestion.svelte'
    import { questions } from '../data/questions'
    import getRandomItem from '../lib/getRandomItem'
</script>

<script lang="ts">
    import { question } from '../lib/stores'

    question.set(getRandomItem(questions))
</script>

<Layout title="Questions">
    <div>
        <p>
            {questions.length} questions about
        </p>
        <h1>Lorem ipsum</h1>

        <RandomQuestion />
    </div>
</Layout>
