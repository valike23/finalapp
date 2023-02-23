<script lang="ts">
	import { onMount } from 'svelte';

	let myApp: any = {};
	let win: any = {};

	onMount(() => {
		win = window;
		myApp = win.L.map('mapid', {
			dragging: !win.L.Browser.mobile,
			tap: !win.L.Browser.mobile
		}).setView([9.082, 8.6753], 6);

		win.L.tileLayer('https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png', {
			attribution: '<a href="https://www.openstreetmap.org/">OpenStreetMap</a>'
		}).addTo(myApp);
	});
</script>

<div id="wrapper">
	<!-- Header -->
	<header id="header" class="alt">
		<a href="/" class="logo">
			<span><img alt="" class="logo" src="Sportsmanager_logo.png" /></span></a
		>
		<nav>
			<a href="#menu">Menu</a>
		</nav>
	</header>
	<!-- Menu -->
	<nav id="menu">
		<ul class="links">
			<li><a href="/">Home</a></li>
			<li><a href="#two">Try out for free</a></li>
			<li><a href="#rankings">Rankings</a></li>
			<li>
				<a href="/">Software Downloads</a>
			</li>
		</ul>
		<ul class="actions stacked">
            <li><a href="/accounts/register" class="button primary fit">Get Started</a></li>
            <li><a href="/accounts/login" class="button fit">Log In</a></li>
        </ul>
        
	</nav>

	<!-- Banner -->
	<section id="banner" class="major">
		<div class="inner">
			<header class="major">
				<h1>SOFTWARE FOR PROFESSIONAL EVENT MANAGEMENT</h1>
			</header>
			<div class="content">
				<p>
					ONLINE REGISTRATION, ON-SITE-SUPPORT, ACCREDITATION, MULTIPLE TOURNAMENT SYSTEMS, TIMING
					AND SCORING, LIVE RESULTS AND STREAMS, VIDEO REVIEW, TV-INTERFACES, CLICKER AND SCORING
					DEVICES, APPS, CUSTOM DEVELOPMENT, AND LOTS OF OTHER SYSTEMS AND SERVICES
				</p>
				<ul class="actions">
					<li><a href="/ " class="button next scrolly">BROWSE EVENTS</a></li>
				</ul>
			</div>
		</div>
	</section>

	<!-- Main -->
	<div>
		<div id="mapid" />

		<!-- One -->
		<section id="one" class="tiles">
			<article id="appinstall">
				<span class="image">
					<img
						src="https://www.sportdata.org/mainpage2018/images/complete-sportsid-min.png"
						alt=""
					/>
				</span>
				<header class="major">
					<h3>Event and Ranking App</h3>
				</header>
			</article>
			<article>
				<span class="image">
					<img src="https://www.sportdata.org/mainpage2018/images/wkf.jpg" alt="" />
				</span>
				<header class="major">
					<h3>
						<a href="/" class="link"
							>WKF</a
						>
					</h3>
					<p>WORLD KARATE FEDERATION EVENTS</p>
				</header>
			</article>
			<article>
				<span class="image">
					<img src="https://www.sportdata.org/setglimg/slider/boxing/aiba.jpg" alt="" />
				</span>
				<header class="major">
					<h3>
						<a
							href="/"
							class="link">IBA</a
						>
					</h3>
					<p>International Boxing Association</p>
				</header>
			</article>
			<article>
				<span class="image">
					<img src="https://www.sportdata.org/mainpage2018/images/karate.jpg" alt="" />
				</span>
				<header class="major">
					<h3>
						<a
							href="/"
							class="link">KARATE</a
						>
					</h3>
					<p>KARATE EVENTS</p>
				</header>
			</article>

			<article>
				<span class="image">
					<img src="https://www.sportdata.org/mainpage2018/images/judo.jpg" alt="" />
				</span>
				<header class="major">
					<h3>
						<a href="/" class="link"
							>JUDO</a
						>
					</h3>
					<p>JUDO EVENTS</p>
				</header>
			</article>

			<article>
				<span class="image">
					<img src="https://www.sportdata.org/mainpage2018/images/fijlkamjudo.jpg" alt="" />
				</span>
				<header class="major">
					<h3>
						<a
							href="/"
							class="link">FIJLKAM JUDO</a
						>
					</h3>
					<p>FIJLKAM JUDO EVENTS</p>
				</header>
			</article>
			<article>
				<span class="image">
					<img src="https://www.sportdata.org/mainpage2018/images/fijlkamkarate.jpg" alt="" />
				</span>
				<header class="major">
					<h3>
						<a
							href="/"
							class="link">FIJLKAM KARATE</a
						>
					</h3>
					<p>FIJLKAM KARATE EVENTS</p>
				</header>
			</article>
			<article>
				<span class="image">
					<img src="https://www.sportdata.org/mainpage2018/images/csen.png" alt="" />
				</span>
				<header class="major">
					<h3>
						<a href="/" class="link"
							>CSEN</a
						>
					</h3>
					<p>Centro Sportivo Educativo Nazionale</p>
				</header>
			</article>
			<article>
				<span class="image">
					<img src="https://www.sportdata.org/setglimg/slider/gymnastics/slide1.jpg" alt="" />
				</span>
				<header class="major">
					<h3>
						<a
							href="/"
							class="link">Gymnastics</a
						>
					</h3>
					<p>Artistic, Rhythmic, Trampoline, Acrobatic, Aerobic, Rope Skipping, ...</p>
				</header>
			</article>
			<article>
				<span class="image">
					<img src="https://www.sportdata.org/mainpage2018/images/esport-main.jpg" alt="" />
				</span>
				<header class="major">
					<h3><a href="/" class="link">E-Sports Events</a></h3>
					<p>E-Sports Events</p>
				</header>
			</article>
		</section>

		<!-- Two -->
		<section id="two">
			<div class="inner">
				<header class="major">
					<h2>TRY OUT FOR FREE</h2>
				</header>
				<p>
					SportManager allows teams, clubs and event managers to enter, administrate and monitor
					registrations quickly and comfortable! SportManager offers you the chance to manage all
					event activities paperless.
				</p>
				<ul class="actions">
					<li><a href="/" class="button next">TEST SYSTEM</a></li>
				</ul>
			</div>
		</section>

		<section id="rankings">
			<div class="inner">
				<header class="major">
					<h2>RANKINGS</h2>
				</header>
				<p>
					You are looking for a custom ranking system for your Federation, Club or Organization? We
					can provide a feature rich and adjustable ranking system for your events, in order to save
					you time and money.
				</p>
				<ul class="actions">
					<li>
						<a href="/product/custom-ranking-system" class="button next">Need a custom ranking?</a>
					</li>
				</ul>
				<ul class="actions stacked">
					<li>
						<a href="https://www.sportdata.org/etournament.html#rankings" class="button fit"
							>E-Tournament Rankings</a
						>
					</li>
					<li>
						<a href="http://setopen.sportdata.org/wkfranking" class="button primary  fit"
							>WKF (World Karate Federation)</a
						>
					</li>
					<li>
						<a href="http://setopen.sportdata.org/wakoranking" class="button fit"
							>WAKO (World Association of Kickboxing Organizations)</a
						>
					</li>
					<li>
						<a href="http://setopen.sportdata.org/mmaranking" class="button primary fit">GAMMA</a>
					</li>
					<li>
						<a href="http://setopen.sportdata.org/wakopanamranking" class="button fit">WAKO PANAM</a
						>
					</li>
					<li>
						<a href="http://setopen.sportdata.org/csencinofiliaranking" class="button fit"
							>CSEN Cinofilia</a
						>
					</li>
				</ul>
			</div>
		</section>
	</div>
</div>

<style>
	.logo {
		width: 20em;
		height: 6 em;
	}
	#mapid {
		height: 500px;
	}
</style>
