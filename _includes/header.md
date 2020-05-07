<header>
	<div class="container">
		<div class="burger-box"></div>
		<div class="title">
			<h1><a href="/">Axel Buob</a></h1>
		</div>
		<div class="search-box"></div>
	</div>
	<nav>
	  <ul>
	  	{% for link in site.data.navigation.header %}
			<li><a href="{{ link.href }}">{{ link.name }}</a></li>
	  	{% endfor %}
	  </ul>
	</nav>
</header>
