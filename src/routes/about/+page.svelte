<script>
	const members = [
		'kimnh-0823',
		'kimyvgy',
		'toanpv-0639',
		'ntduc',
		'hungnm',
		'manhbq-2536',
		'trungtd',
		'ductt-0524',
		'bachdx-1307',
		'thinhnt-3039',
		'loitv-2609',
		'linhdb-2149',
		'trong123',
		'viet',
		'tuyen',
		'kimyvgy2',
		'tuyen3'
	];
</script>

<svelte:head>
	<title>About</title>
	<meta name="description" content="About this app" />
</svelte:head>

<div class="text-column">
	<h1>About this app</h1>

	<p>
		This is a <a href="https://kit.svelte.dev">SvelteKit</a> app. You can make your own by typing the
		following into your command line and following the prompts:
	</p>

	<pre>npm create svelte@latest</pre>

	<p>
		The page you're looking at is purely static HTML, with no client-side interactivity needed.
		Because of that, we don't need to load any JavaScript. Try viewing the page's source, or opening
		the devtools network panel and reloading.
	</p>

	<p>
		The <a href="/sverdle">Sverdle</a> page illustrates SvelteKit's data loading and form handling. Try
		using it with JavaScript disabled!
	</p>

	<ul>
		{#each members as path}
			<li>
				<a href={`/${path}`}>{path}</a>
			</li>
		{/each}
	</ul>
</div>
