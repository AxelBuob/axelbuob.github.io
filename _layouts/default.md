<!DOCTYPE html>
<html lang="en">
<head>
	<meta charset="UTF-8">
	<meta name="viewport" content="width=device-width, initial-scale=1">
	<title>{{ page.title }}</title>
	<link rel="stylesheet" href="{{ 'assets/css/screen.css' | relative_url }}">
	<script src="https://www.google.com/recaptcha/api.js" async defer></script>
	{% feed_meta %}
	{% seo %}
</head>
<body>
	{% include header.md %}
	<main>{{ content }}</main>
	{% include footer.md %}
</body>
</html>