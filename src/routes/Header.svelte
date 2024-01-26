<script>
	import logo from '$lib/sammy.svg';
</script>

<nav class="mainNav">
	<div class="mainNav__logo"><a href="/" class="logo"><img src={logo} alt="sammy" />SAMMY</a></div>
	<div class="mainNav__links">
		<a href="#projects" class="mainNav__link">Projects</a>
		<a href="#language" class="mainNav__link">life</a>
		<a href="https://t.me/smllmy" class="mainNav__link">Contacts</a>
		<a href="#about" class="mainNav__link">About</a>
	</div>
	<div class="mainNav__icon">
		<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
			<g data-name="Layer 2" fill="#9197AE">
				<g data-name="menu-2">
					<rect width="24" height="24" transform="rotate(180 12 12)" opacity="0" />
					<circle cx="4" cy="12" r="1" />
					<rect x="7" y="11" width="14" height="2" rx=".94" ry=".94" />
					<rect x="3" y="16" width="18" height="2" rx=".94" ry=".94" />
					<rect x="3" y="6" width="18" height="2" rx=".94" ry=".94" />
				</g>
			</g>
		</svg>
	</div>
</nav>

<style>
	* {
		margin: 0;
		padding: 0;
		list-style: none;
		border: 0;
		outline: 0;
		-webkit-tap-highlight-color: transparent;
		text-decoration: none;
		color: inherit;
		box-sizing: border-box;
	}
	*:focus {
		outline: 0;
	}

	.mainNav {
		width: 100%;
		height: 110px;
		position: absolute;
		z-index: 1;
		display: flex;
		justify-content: space-between;
		align-items: center;
		color: #9197ae;
		text-transform: uppercase;
		padding: 0 40px;
		font-family: 'Poppins', sans-serif;
	}
	@media screen and (max-width: 799px) {
		.mainNav {
			padding: 0 20px;
		}
	}
	.mainNav__logo {
		font-weight: 800;
		letter-spacing: 1px;
		font-size: 18px;
	}

	.mainNav__links {
		display: flex;
	}
	@media screen and (max-width: 799px) {
		.mainNav__links {
			display: none;
		}
	}
	.mainNav__link {
		letter-spacing: 1px;
		font-size: 14px;
		margin-left: 20px;
		font-weight: 700;
		border-radius: 2px;
		box-shadow: 0px -10px 0px rgba(255, 255, 255, 0.5) inset;
		transition:
			all 0.4s ease,
			transform 0.3s ease;
		padding: 2px 4px;
		transform: translateY(0px);
	}
	.mainNav__link:hover {
		transform: translateY(-5px);
		box-shadow: inset 0px -25px 0px white;
	}

	.mainNav__icon {
		background-image: url($lib/menu-regular-24.png);
		width: 32px;
		height: 32px;
		background-size: contain;
		background-repeat: no-repeat;
		background-position: center;
		display: none;
	}
	@media screen and (max-width: 799px) {
		.mainNav__icon {
			display: block;
		}
	}

	.logo {
		top: auto;
		display: flex;
	}

	.logo img {
		height: 3rem;
		width: 3rem;
		margin-top: -0.7rem;
	}
</style>
