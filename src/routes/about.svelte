<script lang="ts">
</script>

<!-- about -->

<header class="about">
	<div class="about-content">
		<article class="about-text">
			<p class="about-preTitle">nature</p>
			<h2 class="about-title">behind the mountains</h2>
			<p class="about-description">
				Far far away, behind the word mountains, far from the countries Vokalia and Consonantia,
				there live the blind texts.
			</p>
			<button class="cta">know more</button>
		</article>

		<figure class="about-image">
			<img
				src="https://images.unsplash.com/photo-1520856707909-75c4048cc858?ixlib=rb-1.2.1&auto=format&fit=crop&w=1534&q=80"
				alt=""
			/>
		</figure>
	</div>
</header>

<!-- about end -->

<style>
	/* about css*/

	.about {
		width: 100%;
		height: 100%;
		margin-top: 100px;
		position: relative;
		padding: 40px 40px;
		background-image: linear-gradient(to top, #accbee 0%, #e7f0fd 100%);
		overflow: hidden;
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
		background-color: rgba(255, 255, 255, 0.2);
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
		background-color: rgba(255, 255, 255, 0.5);
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
		width: 60%;
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
			right: -6%;
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
	.cta {
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
	.cta:hover {
		border: 1px solid rgba(99, 116, 152, 0.1);
		box-shadow: inset 0px -80px 0px rgba(99, 116, 152, 0.1);
		transform: translateY(-5px);
	}
	@media screen and (max-width: 799px) {
		.cta {
			margin-top: 16px;
		}
	}

	/* about css end */
</style>
