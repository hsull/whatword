<script lang="ts">
    import { fade } from 'svelte/transition';

    export let word: string | undefined;
</script>

<div id="answer-modal">
<h1 > The Answer Is:</h1>
<div class="answer-wrapper">{word}</div>
</div>

<style>
    #answer-modal {
        width: 100%;
        text-align: center;
    }

    .answer-wrapper {
        color: var(--color-accent-light);
        text-align: center;
        text-transform: uppercase;
        font-size: calc(3em + 2vw);
        font-weight: 800;
    }

    @media (max-width: 350px) {
        .answer-wrapper {
            font-size: 2em;
        }
    }
</style>