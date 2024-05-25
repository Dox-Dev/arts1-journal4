<script lang="ts">
	import '../app.postcss';

	// Floating UI for Popups
	import { computePosition, autoUpdate, flip, shift, offset, arrow } from '@floating-ui/dom';
	import { storePopup } from '@skeletonlabs/skeleton';
	storePopup.set({ computePosition, autoUpdate, flip, shift, offset, arrow });

	import { AppBar } from '@skeletonlabs/skeleton';

	let innerWidth = 0;
	let HIDE_SOCMED_TEXT_THRESHOLD = 770; // measured in px
</script>

<svelte:window bind:innerWidth />

<AppBar>
	<svelte:fragment slot="lead"><i class="fa-solid fa-paintbrush"></i></svelte:fragment>
	Artist Freedom Wall
	<svelte:fragment slot="trail">
		{#if innerWidth > HIDE_SOCMED_TEXT_THRESHOLD}
			<a
			class="btn btn-sm variant-ghost-surface"
			href="https://github.com/Dox-Dev/arts1-journal4"
			target="_blank"
			rel="noreferrer"
			>
				<i class="fa-brands fa-github pr-2"/> GitHub Repository
			</a>
			<a
				class="btn btn-sm variant-ghost-surface"
				href="https://www.facebook.com/joseellis.caluag/"
				target="_blank"
				rel="noreferrer"
			>
				<i class="fa-brands fa-facebook pr-2"/> Jose Ellis Miguel Caluag
			</a>
		{:else}
			<a
			class="btn-icon variant-ghost-surface"
			href="https://github.com/Dox-Dev/arts1-journal4"
			target="_blank"
			rel="noreferrer"
			>
				<i class="fa-brands fa-github"/>
			</a>
			<a
				class="btn-icon variant-ghost-surface"
				href="https://www.facebook.com/joseellis.caluag/"
				target="_blank"
				rel="noreferrer"
			>
				<i class="fa-brands fa-facebook"/>
			</a>
		{/if}
	</svelte:fragment>
</AppBar>

<slot />
