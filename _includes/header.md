<header class="header">
	<div class="container">
		<h1 class="header_title">
			<a href="/">
				<span class="header_title_short">AB</span>
				<span class="header_title_full">Axel Buob</span>
			</a>
		</h1>
		<div id="navbar_toggle" class="navbar_toggle">
				<div class="navbar_toggle_inner"></div>
				<div class="navbar_toggle_inner"></div>
		</div>
		<nav id="navbar" class="navbar">
			<ul>
				{% for link in site.data.navigation.header %}
				<li><a class="navbar_link" href="{{ link.href }}">{{ link.name }}</a></li>
				{% endfor %}
			</ul>
		</nav>
	</div>
</header>
