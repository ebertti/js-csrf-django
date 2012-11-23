js-csrf-django
==============

Simple javascript to make easy to make POST with AJAX using Django. Based on django documentation.

Installation
------------

1. Add ``CsrfViewMiddleware`` in your  ``MIDDLEWARE_CLASSES`` in ``settings.py`` file of your project. 
``` python
MIDDLEWARE_CLASSES = (
	...
	'django.middleware.csrf.CsrfViewMiddleware',
	...
)
```

2. Add the javascript file  ``https://raw.github.com/ebertti/js-csrf-django/master/csrf.js`` in the ``head`` of your html page, rather in yout ``base.html``, after jQuery file:
```html

	<html>
		<head>
			<script src="//ajax.googleapis.com/ajax/libs/jquery/1.8.3/jquery.min.js"></script>
			<scripr scr="https://raw.github.com/ebertti/js-csrf-django/master/csrf.js"></script>
		</head>
	</html>
```
3. Now you can make your AJAX request using POST.
