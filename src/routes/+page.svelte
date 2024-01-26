<script lang="ts">
	import person from '$lib/person.png';
	import geda from '$lib/geda.jpg';
	import chewata from '$lib/chewata.jpg';
	import fact from '$lib/fact.jpg';
	import vici from '$lib/vici.jpg';
</script>

<!-- floating button -->
<div class="floating">
	<a class="bg_links social github" href="https://www.github.com" target="_blank">
		<span class="icon"></span>
	</a>
	<a class="bg_links social instagram" href="https://www.instagram.com" target="_blank">
		<span class="icon"></span>
	</a>
	<a class="bg_links social telegram" href="https://t.me/smllmyh" target="_blank">
		<span class="icon"></span>
	</a>
	<a class="bg_links logo"></a>
</div>
<!-- floating button end -->

<!-- landing page -->
<div class="person">
	<div class="gradient-border"><img src={person} alt="sammy" /></div>
	<main class="container">
		<p>Hello 👋 I'm</p>
		<section class="animation">
			<div class="first"><div>SAMUEL A. HAILE</div></div>
			<div class="second"><div>Web Developer</div></div>
			<div class="third"><div>Frontender</div></div>
		</section>
	</main>
</div>

<!-- landing page end -->

<!-- project -->
<div id="projects" class="projects">
	<div class="bx-container">
		<div class="box">
			<div class="imgBx">
				<img src={geda} alt="geda" />
			</div>
			<div class="content">
				<div>
					<a href="https://github.com/SMLLMYH"
						><h2>Geda Store</h2>
						<p>
							Geda store is one of the biggest cloth shopping platform in ethiopia where you can buy
							any clothes from casual to cultural clothes.
						</p></a
					>
				</div>
			</div>
		</div>
		<div class="box">
			<div class="imgBx">
				<img src={chewata} alt="chewata" />
			</div>
			<div class="content">
				<div>
					<a href="https://github.com/SMLLMYH"
						><h2>Chewata</h2>
						<p>
							chewata is an online platform where you can find different type of games in play while
							enjoying your time. let's go!
						</p></a
					>
				</div>
			</div>
		</div>
		<div class="box">
			<div class="imgBx">
				<img src={fact} alt="fact" />
			</div>
			<div class="content">
				<div>
					<a href="https://github.com/SMLLMYH"
						><h2>Fun facts</h2>
						<p>The place where you find unlimited random facts from all over the world</p></a
					>
				</div>
			</div>
		</div>
		<div class="box">
			<div class="imgBx">
				<img src={vici} alt="vici" />
			</div>
			<div class="content">
				<div>
					<a href="https://github.com/SMLLMYH"
						><h2>VICI Movies - <br class="on-prog" /> on progress</h2>
						<p>Free online movie streaming website with vareity of movies and series</p></a
					>
				</div>
			</div>
		</div>
	</div>
</div>

<!-- project end -->

<!-- language -->
<div class="language" id="language">
	<h2>Language</h2>
	<div class="lang-coll">
		<div class="svelte-circle-grad">
			<div class="svelte">
				<img
					src="https://upload.wikimedia.org/wikipedia/commons/1/1b/Svelte_Logo.svg"
					alt="svelte"
				/>
				<h2 class="sv-h2">Sveltekit</h2>
				<a href="https://www.svelte.com" target="_blank">try me</a>
			</div>
		</div>
		<div class="html-circle-grad">
			<div class="html">
				<img src="https://upload.wikimedia.org/wikipedia/commons/3/38/HTML5_Badge.svg" alt="html" />
				<h2 class="sv-h2">HTML</h2>
				<a href="https://www.html.com" target="_blank">try me</a>
			</div>
		</div>

		<div class="js-circle-grad">
			<div class="js">
				<img
					src="https://upload.wikimedia.org/wikipedia/commons/9/99/Unofficial_JavaScript_logo_2.svg"
					alt="js"
				/>
				<h2 class="sv-h2">JavaScript</h2>
				<a href="https://www.js.com" target="_blank">try me</a>
			</div>
		</div>
	</div>
</div>

<!-- language end -->

<!-- about -->

<header class="about" id="about">
	<div class="about-content">
		<article class="about-text">
			<p class="about-preTitle">About</p>
			<h2 class="about-title"><span>Samuel A. HAILE</span></h2>
			<p class="about-description">
				<span
					>My name is SAMUEL ALEMAYEHU HAILE. I live in Adama,Nazret and I'm 3rd year software
					enginering studet at Adama Science and Technology University (ASTU). I've worked in so
					many projects that I even lost the number to count so, If you need anything you can
					contact me anytime. <br /> <br /> KALAS!
				</span>
			</p>
			<button class="contact-btn"
				><a href="https://t.me/smllmyh" target="_blank">contact me</a></button
			>
		</article>

		<figure class="about-image">
			<img src={person} alt="" />
		</figure>
	</div>
</header>

<!-- about end -->

<style>
	/* floating button css */
	.floating {
		position: fixed;
		z-index: 10;
		bottom: 35px;
		right: 40px;
		width: 40px;
		height: 40px;
		display: flex;
		justify-content: flex-end;
		align-items: flex-end;
		transition: all 0.2s ease;
	}
	.floating .bg_links {
		width: 45px;
		height: 45px;
		border-radius: 100%;
		display: flex;
		justify-content: center;
		align-items: center;
		background-color: rgba(0, 0, 0, 0.2);
		border-radius: 100%;
		backdrop-filter: blur(5px);
		position: absolute;
	}
	.floating .logo {
		width: 50px;
		height: 50px;
		z-index: 9;
		background-image: url($lib/sammy.svg);
		background-size: 100%;
		background-repeat: no-repeat;
		background-position: 0;

		opacity: 0.9;
		transition: all 1s 0.2s ease;
		bottom: 0;
		right: 0;
	}
	.floating .social {
		opacity: 0;
		right: 0;
		bottom: 0;
	}

	.floating .social .icon {
		width: 100%;
		height: 100%;
		background-size: 20px;
		background-repeat: no-repeat;
		background-position: center;
		background-color: transparent;
		display: flex;
		transition:
			all 0.2s ease,
			background-color 0.4s ease;
		opacity: 0;
		border-radius: 100%;
	}
	.floating .social.github {
		transition: all 0.8s ease;
	}
	.floating .social.github .icon {
		background-image: url($lib/social/github.svg);
	}
	.floating .social.github .icon:hover {
		background-color: #6d6d6d;
	}
	.floating .social.instagram {
		transition: all 0.3s ease;
	}
	.floating .social.instagram .icon {
		background-image: url($lib/social/instagram.svg);
	}
	.floating .social.instagram .icon:hover {
		background-color: #ff6464;
	}
	.floating .social.telegram {
		transition: all 0.8s ease;
	}
	.floating .social.telegram .icon {
		background-image: url($lib/social/telegram.svg);
	}
	.floating .social.telegram .icon:hover {
		background-color: #0051ff;
	}
	.floating:hover {
		width: 105px;
		height: 105px;
		transition: all 0.6s cubic-bezier(0.64, 0.01, 0.07, 1.65);
	}
	.floating:hover .logo {
		opacity: 1;
		transition: all 0.6s ease;
	}
	.floating:hover .social {
		opacity: 1;
	}
	.floating:hover .social .icon {
		opacity: 0.9;
	}
	.floating:hover .social:hover {
		background-size: 28px;
	}
	.floating:hover .social:hover .icon {
		background-size: 65%;
		opacity: 1;
	}
	.floating:hover .social.github {
		right: 0;
		bottom: calc(100% - 40px);
		transition: all 0.3s 0s cubic-bezier(0.64, 0.01, 0.07, 1.65);
	}
	.floating:hover .social.instagram {
		bottom: 45%;
		right: 45%;
		transition: all 0.3s 0.15s cubic-bezier(0.64, 0.01, 0.07, 1.65);
	}
	.floating:hover .social.telegram {
		bottom: 0;
		right: calc(100% - 40px);
		transition: all 0.3s 0.25s cubic-bezier(0.64, 0.01, 0.07, 1.65);
	}

	/* floating button css end */

	/* landing page css */
	.person {
		position: relative;
		justify-content: space-around;
		display: flex;
		margin-top: 4rem;
	}

	.gradient-border img {
		position: relative;
		display: flex;
		justify-content: center;
		align-items: center;
		width: 280px;
		height: 280px;
		font-family: 'Poppins', sans-serif;
		font-size: 2.5rem;
		text-transform: uppercase;
		color: white;
		background: var(--gradient-02);
		border-radius: 50%;
	}
	.gradient-border {
		--border-width: 3px;
		--radius: 50%;
		float: left;
		position: relative;
		display: flex;
		justify-content: center;
		align-items: center;
		width: 280px;
		height: 280px;

		color: white;
		background: transparent;
		border-radius: 50%;
		margin-top: 5rem;
	}
	.gradient-border::after {
		position: absolute;
		content: '';
		top: calc(-1 * var(--border-width));
		left: calc(-1 * var(--border-width));
		z-index: -1;
		width: calc(100% + var(--border-width) * 2);
		height: calc(100% + var(--border-width) * 2);
		background: linear-gradient(
			60deg,
			#5f86f2,
			#a65ff2,
			#f25fd0,
			#f25f61,
			#f2cb5f,
			#abf25f,
			#5ff281,
			#5ff2f0
		);
		background-size: 300% 300%;
		background-position: 0 50%;
		border-radius: calc(2 * var(--radius));
		animation: moveGradient 4s alternate infinite;
	}
	@keyframes moveGradient {
		50% {
			background-position: 100% 50%;
		}
	}

	.container {
		font-family: 'Poppins', sans-serif;
		color: #000000;
		font-size: 2.26rem;
		text-transform: uppercase;
		height: 100vh;
		display: flex;
		align-items: center;
		justify-content: center;
		margin-top: -50px;
	}

	.animation {
		height: 50px;
		overflow: hidden;
		margin-left: 1rem;
	}

	.animation > div > div {
		padding: 0.25rem 0.75rem;
		height: 2.81rem;
		margin-bottom: 2.81rem;
		display: inline-block;
	}

	.animation div:first-child {
		animation: text-animation 8s infinite;
	}

	.first div {
		background-color: #20a7d8;
	}
	.second div {
		background-color: #cd921e;
	}
	.third div {
		background-color: #c10528;
	}

	@keyframes text-animation {
		0% {
			margin-top: 0;
		}
		10% {
			margin-top: 0;
		}
		20% {
			margin-top: -5.92rem;
		}
		30% {
			margin-top: -5.92rem;
		}
		40% {
			margin-top: -11.64rem;
		}
		60% {
			margin-top: -11.64rem;
		}
		70% {
			margin-top: -5.62rem;
		}
		80% {
			margin-top: -5.62rem;
		}
		90% {
			margin-top: 0;
		}
		100% {
			margin-top: 0;
		}
	}

	/* landing page css end */

	/* project css*/

	.on-prog {
		font-size: 10px;
		color: red;
	}
	.projects {
		justify-content: center;
		align-items: center;
		display: flex;
		position: relative;
		overflow: hidden;
		margin-top: 1rem;
	}
	.bx-container {
		position: relative;
		width: 1160px;
		display: flex;
		justify-content: center;
		flex-wrap: wrap;
		transform-style: preserve-3d;
		perspective: 500px;
		margin: auto;
	}
	.bx-container .box {
		position: relative;
		width: 220px;
		height: 220px;
		background: #000;
		transition: 0.5s;
		transform-style: preserve-3d;
		overflow: hidden;
		margin-right: 15px;
		margin-top: 45px;
		border-radius: 5px;
	}
	.bx-container:hover .box {
		transform: rotateY(25deg);
	}
	.bx-container .box:hover ~ .box {
		transform: rotateY(-25deg);
	}
	.bx-container .box:hover {
		transform: rotateY(0deg) scale(1.25);
		z-index: 1;
		box-shadow: 0 25px 40px rgba(0, 0, 0, 0.5);
	}
	.bx-container .box .imgBx {
		position: absolute;
		top: 0;
		left: 0;
		width: 100%;
		height: 100%;
	}
	.bx-container .box .imgBx:before {
		content: '';
		position: absolute;
		top: 0;
		left: 0;
		width: 100%;
		height: 100%;
		background: linear-gradient(180deg, rgb(0, 195, 255), #000);
		z-index: 1;
		opacity: 0;
		transition: 1.5s;
		mix-blend-mode: multiply;
	}
	.bx-container .box:hover .imgBx:before {
		opacity: 1;
	}
	.bx-container .box .imgBx img {
		position: absolute;
		top: 0;
		left: 0;
		width: 100%;
		height: 100%;
		object-fit: cover;
	}
	.bx-container .box .content {
		position: absolute;
		top: 0;
		left: 0;
		width: 100%;
		height: 100%;
		z-index: 1;
		display: flex;
		padding: 20px;
		align-items: flex-end;
		box-sizing: border-box;
	}
	.bx-container .box .content h2 {
		color: #fff;
		transition: 0.5s;
		text-transform: uppercase;
		margin-bottom: 5px;
		font-size: 20px;
		transform: translateY(200px);
		transition-delay: 0.1s;
	}
	.bx-container .box:hover .content h2 {
		transform: translateY(0px);
	}
	.bx-container .box .content p {
		color: #fff;
		transition: 0.5s;
		font-size: 14px;
		transform: translateY(200px);
		transition-delay: 0.2s;
	}
	.bx-container .box:hover .content p {
		transform: translateY(0px);
	}

	/* project css end */

	/* language css */
	.language {
		display: flex;
		justify-content: center;
		align-items: center;
		box-sizing: border-box;
		gap: 5px;

		flex-direction: column;
		padding: 0;
		margin-top: 150px;
	}

	.language h2 {
		color: #000000;
		text-transform: uppercase;
	}

	.lang-coll {
		display: flex;
		justify-content: center;
		align-items: center;
		box-sizing: border-box;
		gap: 50px;
	}
	.svelte-circle-grad {
		position: relative;
		width: 80px;
		height: 80px;
		background: transparent;
		border-radius: 50%;
		overflow: hidden;
	}
	.svelte-circle-grad::before {
		content: '';
		position: absolute;
		inset: -1px 35px;
		background: linear-gradient(to top, #ffffff 0%, #ff4800 150%);
		transition: 0.5s;
		animation: animate 4s linear infinite;
	}

	.svelte-circle-grad:hover::before {
		inset: -20px 0px;
	}

	@keyframes animate {
		0% {
			transform: rotate(0deg);
		}
		100% {
			transform: rotate(360deg);
		}
	}

	.svelte-circle-grad::after {
		content: '';
		position: absolute;
		inset: 3px;
		background: #ff4800;
		border-radius: 50%;
		z-index: 1;
	}

	.svelte {
		position: absolute;
		inset: 3px;
		border: 1px solid rgba(0, 0, 0, 0.301);
		z-index: 3;
		border-radius: 50%;
		overflow: hidden;
		display: flex;
		justify-content: center;
		align-items: center;
		flex-direction: column;
	}

	.svelte img {
		position: absolute;
		top: 0;
		left: 0;
		width: 100%;
		height: 100%;
		transition: 0.5s;
		pointer-events: none;
		z-index: 3;
	}

	.svelte-circle-grad:hover .svelte img {
		opacity: 0;
	}

	.svelte h2 {
		position: relative;
		font-size: 0.6rem;
		color: #fff;
		font-weight: 600;
		letter-spacing: 0.05em;
		text-transform: uppercase;
	}

	.svelte a {
		position: relative;
		margin-top: 0.5px;
		padding: 2.5px 5px;
		background: #fff;
		color: #070a1c;
		border-radius: 25px;
		font-weight: 500;
		font-size: 0.1em;
		text-decoration: none;
		transition: 0.5s;
		text-transform: uppercase;
	}

	.svelte a:hover {
		letter-spacing: 0.2em;
	}

	.html-circle-grad {
		position: relative;
		width: 80px;
		height: 80px;
		display: flex;
		margin-left: 1px;
		background: transparent;
		border-radius: 50%;
		overflow: hidden;
	}
	.html-circle-grad::before {
		content: '';
		position: absolute;
		inset: -1px 35px;
		background: linear-gradient(to top, #ffffff 0%, #ff1e00 150%);
		transition: 0.5s;
		animation: animate 4s linear infinite;
	}

	.html-circle-grad:hover::before {
		inset: -20px 0px;
	}

	@keyframes animate {
		0% {
			transform: rotate(0deg);
		}
		100% {
			transform: rotate(360deg);
		}
	}

	.html-circle-grad::after {
		content: '';
		position: absolute;
		inset: 3px;
		background: #e34f26;
		border-radius: 50%;
		z-index: 1;
	}

	.html {
		position: absolute;
		inset: 3px;
		border: 1px solid rgba(0, 0, 0, 0.201);
		z-index: 3;
		border-radius: 50%;
		overflow: hidden;
		display: flex;
		justify-content: center;
		align-items: center;
		flex-direction: column;
	}

	.html img {
		position: absolute;
		top: 0;
		left: 0;
		width: 100%;
		height: 100%;
		transition: 0.5s;
		pointer-events: none;
		z-index: 3;
	}

	.html-circle-grad:hover .html img {
		opacity: 0;
	}

	.html h2 {
		position: relative;
		font-size: 0.6rem;
		color: #fff;
		font-weight: 600;
		letter-spacing: 0.05em;
		text-transform: uppercase;
	}

	.html a {
		position: relative;
		margin-top: 0.5px;
		padding: 2.5px 5px;
		background: #fff;
		color: #070a1c;
		border-radius: 25px;
		font-weight: 500;
		font-size: 0.1em;
		text-decoration: none;
		transition: 0.5s;
		text-transform: uppercase;
	}

	.html a:hover {
		letter-spacing: 0.2em;
	}

	.js-circle-grad {
		position: relative;
		width: 80px;
		height: 80px;
		display: flex;
		margin-left: 1px;
		background: transparent;
		border-radius: 50%;
		overflow: hidden;
	}
	.js-circle-grad::before {
		content: '';
		position: absolute;
		inset: -1px 35px;
		background: linear-gradient(to top, #000000 0%, #f7e018 100%);
		transition: 0.5s;
		animation: animate 4s linear infinite;
	}

	.js-circle-grad:hover::before {
		inset: -20px 0px;
	}

	@keyframes animate {
		0% {
			transform: rotate(0deg);
		}
		100% {
			transform: rotate(360deg);
		}
	}

	.js-circle-grad::after {
		content: '';
		position: absolute;
		inset: 3px;
		background: #f7e018;
		border-radius: 50%;
		z-index: 1;
	}

	.js {
		position: absolute;
		inset: 3px;
		border: 1px solid #bdaa00;
		z-index: 3;
		border-radius: 50%;
		overflow: hidden;
		display: flex;
		justify-content: center;
		align-items: center;
		flex-direction: column;
	}

	.js img {
		position: absolute;
		top: 0;
		left: 0;
		width: 100%;
		height: 100%;
		transition: 0.5s;
		pointer-events: none;
		z-index: 3;
	}

	.js-circle-grad:hover .js img {
		opacity: 0;
	}

	.js h2 {
		position: relative;
		font-size: 0.6rem;
		color: #000000;
		font-weight: 600;
		letter-spacing: 0.05em;
		text-transform: uppercase;
	}

	.js a {
		position: relative;
		margin-top: 0.5px;
		padding: 2.5px 5px;
		background: #fff;
		color: #070a1c;
		border-radius: 25px;
		font-weight: 500;
		font-size: 0.1em;
		text-decoration: none;
		transition: 0.5s;
		text-transform: uppercase;
	}

	.js a:hover {
		letter-spacing: 0.2em;
	}

	/* language css end*/

	/* about css */
	.about {
		width: 100%;
		height: 100%;

		position: relative;
		padding: 40px 40px;
	}
	@media screen and (max-width: 799px) {
		.about {
			padding: 0 20px;
		}
	}
	.about-content {
		max-width: 1110px;
		min-height: 800px;
		left: 50%;
		transform: translateX(-50%);
		display: flex;
		justify-content: space-between;
		align-items: center;
		position: relative;
	}
	@media screen and (max-width: 799px) {
		.about-content {
			min-height: 500px;
		}
	}
	.about-text {
		z-index: 1;
		color: #637498;
		background-color: rgba(0, 55, 128, 0.2);
		padding: 40px;
		max-width: 620px;
		margin-top: 100px;
		width: 70%;
		backdrop-filter: blur(8px);
		animation: text 0.8s 0.6s ease backwards;
		position: relative;
	}
	.about-text:before {
		content: '';
		position: absolute;
		width: 5px;
		height: 100%;
		background-color: rgba(96, 170, 255, 0.5);
		top: 0;
		left: 0;
		animation: line 0.8s 0.6s ease backwards;
	}
	@keyframes line {
		0% {
			right: 0;
			width: 100%;
			opacity: 0;
		}
	}
	@media screen and (max-width: 799px) {
		.about-text {
			padding: 20px;
			margin: 90px 0 40px 0;
		}
	}
	@keyframes text {
		0% {
			opacity: 0;
			transform: translateX(200px);
		}
	}
	.about-preTitle {
		text-transform: uppercase;
		font-weight: 600;
		letter-spacing: 2px;
		margin-bottom: 16px;
		color: #637498;
	}
	.about-title {
		text-transform: uppercase;
		font-weight: 200;
		letter-spacing: 2px;
		margin-bottom: 24px;
		font-size: 40px;
		color: #637498;
	}
	@media screen and (max-width: 799px) {
		.about-title {
			margin-bottom: 16px;
			font-size: 28px;
		}
	}
	.about-description {
		letter-spacing: 0.5px;
		font-size: 16px;
		line-height: 26px;
	}
	@media screen and (max-width: 799px) {
		.about-description {
			font-size: 14px;
		}
	}
	.about-image {
		right: 0;
		max-width: 600px;
		width: 100%;
		height: 600px;
		transform: translatey(100px);
		position: absolute;
		overflow: hidden;

		animation: image 0.6s 0.2s ease backwards;
	}
	@media screen and (max-width: 799px) {
		.about-image {
			height: 480px;
			width: 70%;
			transform: translatey(80px);
			right: -9%;
		}
	}
	@keyframes image {
		0% {
			opacity: 0;
			transform: translatey(200px);
		}
	}
	.about-image:before,
	.about-image:after {
		content: '';
		position: absolute;
		width: 100%;
		height: 0%;
		top: 100%;
		background-image: linear-gradient(to top, #accbee 0%, #e7f0fd 100%);
		opacity: 1;
		left: 0;
	}
	.about-image:before {
		animation: imageBefore 1s 0.2s ease backwards;
	}
	@keyframes imageBefore {
		0% {
			height: 100%;
			top: 0;
		}
	}
	.about-image:after {
		background-image: linear-gradient(to top, #accbee 0%, #e7f0fd 100%);
		height: 100%;
		top: 0;
		opacity: 0.2;
	}
	.about-image img {
		width: 100%;
		height: 100%;
	}
	.contact-btn {
		padding: 16px 32px;
		color: #637498;
		background-color: transparent;
		border: 1px solid rgba(99, 116, 152, 0.4);
		font-family: 'Raleway', sans-serif;
		text-transform: uppercase;
		letter-spacing: 2px;
		font-weight: 600;
		margin-top: 32px;
		cursor: pointer;
		box-shadow: inset 0px 0px 0px rgba(99, 116, 152, 0.2);
		transition: all 0.4s ease;
	}
	.contact-btn:hover {
		border: 1px solid rgba(99, 116, 152, 0.1);
		box-shadow: inset 0px -80px 0px rgba(99, 116, 152, 0.1);
		transform: translateY(-5px);
	}
	@media screen and (max-width: 799px) {
		.contact-btn {
			margin-top: 16px;
		}
	}
	.contact-btn a {
		color: #637498;
	}

	/* about css end */

	/* scroll reveal css*/

	.about-content span {
		color: hsla(0, 0%, 0%, 0.2);
		background-clip: text;
		background-repeat: no-repeat;
		background-size: 0% 100%;
		background-image: linear-gradient(90deg, #637498, #637498);
		animation: about-content linear forwards;
		animation-timeline: view(y);
	}

	.about-content h2 span {
		animation-range-start: cover 20vh;
		animation-range-end: cover 30vh;
	}

	.about-content p span {
		animation-range-start: cover 22.5vh;
		animation-range-end: cover 50vh;
	}

	@keyframes about-content {
		to {
			background-size: 100% 100%;
		}
	}
	/* scroll reveal css end */
</style>
