<script>
	import welcome from '$lib/images/svelte-welcome.webp';
	import welcome_fallback from '$lib/images/svelte-welcome.png';
</script>

<header>
	<div class="corner">
		<a href="https://kit.svelte.dev" class="menu">
			<img src=https://icon-library.com/images/white-hamburger-menu-icon/white-hamburger-menu-icon-24.jpg alt="SvelteKit" />
		</a>
	</div>

	<div class="welcome">
		<picture>
			<source srcset={welcome} type="image/webp" />
			<img src={welcome_fallback} alt="Welcome" />
		</picture>
	</div>

	<div class="corner">
		<a href="https://github.com/sveltejs/kit">
			<img src=https://cdn-icons-png.flaticon.com/512/8061/8061062.png alt="GitHub" />
		</a>
	</div>
</header>

<style>
	header {
		display: flex;
		justify-content: space-between;
		margin: 20px 30px 0 30px;
	}

	.corner {
		width: 3em;
		height: 3em;
	}

	.corner a {
		display: flex;
		align-items: center;
		justify-content: center;
		width: 100%;
		height: 100%;
	}

	.corner img {
		width: 2em;
		height: 2em;
		object-fit: contain;
	}
	.corner .menu img {
		width: 3em;
		height: 3em;
		object-fit: contain;
	}

	a:hover {
		color: var(--color-theme-1);
	}

	.welcome img {
		width: 100%;
		height: 100%;
		top: 0;
		display: block;
	}
</style>
