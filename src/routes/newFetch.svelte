<script>
	import Error from '$components/Error.svelte';
	import Spinner from '$components/Spinner.svelte';
	import { getData } from '$lib/fetcher';

	let response = getData('https://0nzwp.sse.codesandbox.io/');
</script>

<h1>New Fetch</h1>
{#await $response}
	<Spinner />
{:then data}
	<code>{new Date(data).toTimeString()}</code>
{:catch}
	<Error />
{/await}
