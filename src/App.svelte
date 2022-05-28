<script>
	import 'bulma/bulma.sass';
	import {Button} from '@opentj/jui'
	import Counter from './lib/Counter.svelte'
</script>

<main>
    <h1>Hello Svelte!</h1>
    <Counter/>
    <p/>
    <Button class="is-primary is-rounded"
            style="margin-top: 36px;"
            on:click={() => {
                alert('clicked')
            }}>
    Primary Button</Button>
</main>

<style>
    :root {
        font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen,
        Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
    }

    main {
        text-align: center;
        padding: 1em;
        margin: 0 auto;
    }

    h1 {
        color: #ff3e00;
        text-transform: capitalize;
        font-size: 4rem;
        font-weight: 100;
        line-height: 1.1;
        margin: 2rem auto;
        max-width: 14rem;
    }

    @media (min-width: 480px) {
        h1 {
            max-width: none;
        }
    }
</style>
