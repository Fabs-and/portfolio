<slot />

<style>
	:root {
		--clr-bg: #f9fcfd;
		--clr-accent: blue;
		--clr-secondary: #016aa1;
		--clr-font: black;
		--clr-font-contrast: white;
		--clr-font-contrast-black-bg: white;
		--clr-toggle: gray;
		--clr-hover: #e2e8ec;
		--clr-shadow: #0000001a;
		--size-header: 3rem;
	}

	:global(body) {
		background-color: var(--clr-bg);
		font-family: system-ui;
		color: var(--clr-font);
		margin: 0;
	}

	:global(section) {
		box-sizing: border-box;
		height: calc(100svh - 3.7rem);
		display: flex;
		flex-direction: column;
	}

	:global(a) {
		text-decoration: none;
		color: var(--clr-font);
	}

	:global(.header-icons) {
		display: flex;
		justify-content: center;
		align-items: center;
		background: none;
		color: var(--clr-toggle);
		border: none;
		font: inherit;
		cursor: pointer;
		outline: inherit;
		width: 1.3rem;
		height: 1.3rem;
		padding: 0.3rem;
	}

	:global(.header-icons:hover) {
		background-color: var(--clr-hover);
		border-radius: 6px;
		color: black;
		transition: color 0.3s ease, background-color 0.3s ease;
	}
	:global(.icons) {
		background: none;
		color: var(--clr-toggle);
		border: none;
		padding: 0;
		font: inherit;
		cursor: pointer;
		outline: inherit;
		width: 1.5rem;
		height: 1.5rem;
	}

	:global(.dark) {
		--clr-bg: black;
		--clr-font: white;
		--clr-font-contrast-black-bg: var(--clr-accent);
		--clr-shadow: #cccccc;
	}
</style>
