<header>
	<h1 class="title"><a href="/">Axel Buob</a></h1>
	<div>
		<svg class="icon icon-menu"><use xlink:href="/assets/icons/symbol-defs.svg#icon-menu"></use></svg>
		<span class="name">icon-menu</span>
	</div>
	<nav>
	  <ul>
	  	{% for link in site.data.navigation.header %}
			<li><a href="{{ link.href }}">{{ link.name }}</a></li>
	  	{% endfor %}
	  </ul>
	</nav>
</header>

