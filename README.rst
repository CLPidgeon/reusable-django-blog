Blog

Blog is a reusable blog app for Django

Detailed documentation is in the "docs" directory.

Quick start

Add "reusable_blog" to your INSTALLED_APPS setting like this:

INSTALLED_APPS = (
    ...
    'reusable_blog',
)
Include the polls URL conf in your project urls.py like this:

url(r'^blogs/', include('reusable_blog.urls')),

Run python manage.py migrate to create the blog models.

Add the blogs css::
<link rel="stylesheet" href="{% static "css/blog.css" %}">

Visit http://127.0.0.1:8000/blogs/ to view the blogs you create