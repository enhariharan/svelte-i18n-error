<script>
  import {_, setupI18n} from 'services/i18n';
  export let name;
  setupI18n({ withLocale: 'en' });
</script>

<main>
    <h1>{$_('general.hello')} {name}!</h1>
    <p>{$_('general.body')}</p>
    <!--	<p>Visit the <a href="https://svelte.dev/tutorial">Svelte tutorial</a> to learn how to build Svelte apps.</p>-->
</main>

<style>
    main {
        text-align: center;
        padding: 1em;
        max-width: 240px;
        margin: 0 auto;
    }

    h1 {
        color: #ff3e00;
        text-transform: uppercase;
        font-size: 4em;
        font-weight: 100;
    }

    @media (min-width: 640px) {
        main {
            max-width: none;
        }
    }
</style>