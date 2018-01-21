---
layout: default
title: "My first Blog"
email: abcd@gmail.com
---


<h2>{{ page.title }}</h2>
<p>Recent Blog Posts</p>

<ul>
    {% for post in site.posts %}
        <li>{{ post.date | data_to_string }}
        <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
        </li>
    {% endfor %}
</ul>


<!---
# My first Blog
## Recent blog Posts

{% for post in site.posts %}
{{ post.date | date_to_string }}
{% endfor %}
## have a nice day.
--->
