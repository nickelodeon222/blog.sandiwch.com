---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: base
---
hi! i'm pickelodeons/sandiwch/real name that i don't want to say online! i am (as of 2023) 16 years old and i come from new zealand!

i've been on the internet since i was a small child which may have been bad but who knows

{% for post in site.posts %}
# [{{post.title}}]({{post.url}})
{% if post.author %}##### *{{post.author}}*{% endif %}
{% if post.date %}###### {{post.date | date_to_long_string }} NZT{% endif %}
{{post.excerpt}}
{% if post.excerpt != post.content %}[read more]({{post.url}}){% endif %}
{% endfor %}