<script lang="ts">
	import '../app.css';
	import '@fontsource/bricolage-grotesque/400.css';
	import '@fontsource/bricolage-grotesque/600.css';
	import '@fontsource/inter/400.css';
	import '@fontsource/inter/600.css';
	import BricolageGrotesque400 from '@fontsource/bricolage-grotesque/files/bricolage-grotesque-latin-400-normal.woff2?url'
	import BricolageGrotesque600 from '@fontsource/bricolage-grotesque/files/bricolage-grotesque-latin-600-normal.woff2?url'
	import Inter400 from '@fontsource/inter/files/inter-latin-400-normal.woff2?url'
	import Inter600 from '@fontsource/inter/files/inter-latin-600-normal.woff2?url'

	let { children } = $props();
</script>

<svelte:head>
	<meta name="viewport" content="width=device-width, initial-scale=1.0" />
	<meta http-equiv="x-ua-compatible" content="IE=7" />
	<meta http-equiv="content-type" content="text/html;charset=UTF-8" />
	<link rel="preload" as="font" type="font/woff2" href={BricolageGrotesque400} crossorigin="anonymous" />
	<link rel="preload" as="font" type="font/woff2" href={BricolageGrotesque600} crossorigin="anonymous" />
	<link rel="preload" as="font" type="font/woff2" href={Inter400} crossorigin="anonymous" />
	<link rel="preload" as="font" type="font/woff2" href={Inter600} crossorigin="anonymous" />
</svelte:head>

<div class="mx-auto flex min-h-dvh max-w-4xl flex-col px-6 py-12 md:py-20">
	{@render children()}
</div>

<style lang="postcss">
	@reference "tailwindcss";
	
	:global(body) {
		@apply bg-zinc-900 text-zinc-300;
	}
</style>
