---
layout  : name
title   : Home
section : Home
feed    : /atom.xml
---

![Welcome](/images/drawing.png){:title="Jennifer Carrot-Lee"}

Thank you for visiting. I am a graduate student in my late 20s studying computer science in Ottawa, Canada. I created this blog with the intention of becoming a more productive outlet for sharing and learning. I was born and grew up in Indonesia. Things that make me happy are: my old teddy bear, the spring season, minimalist lifestyle, piano, gemstones and crystals. I also love to ponder about astrology and philosophy.

Blog [![Feed icon](/images/rss.png){:title="Feedburner" .right}](http://feeds.feedburner.com/rosebery)
=======================================================================================================

{% for post in site.posts limit:5 %}
<div class="section list">
  <h1>{{ post.date | date_to_string }}</h1>
  <p class="line">
    <a class="title" href="{{ post.url }}">{{ post.title }}</a>
  </p>
  <p class="excerpt">
	{% if post.excerpt %}
	  {{ post.excerpt }}
    {% else %}
      {{ post.content | html_truncate }}
    {% endif %}
  </p>
</div>
{% endfor %}

<p>
<a href="/archives/">Older Posts &rarr;</a>
</p>

+-- {.section}
[Twitter](http://twitter.com/jliyi)
====================================

Contacting Twitter... 
{:#twitter_update_list }

=--

+-- {.section}
[Delicious](http://www.delicious.com/leecarrot)
===============================================
<script type="text/javascript" src="http://feeds.delicious.com/v2/js/leecarrot?title=&count=5&sort=date&tags&extended"> </script>

=--

+-- {.section}
Interweb
========
- [Tumblr](http://leecarrot.tumblr.com)
- [Google Reader](http://www.google.com/reader/shared/leeCarrot)
- [Facebook](http://facebook.com/leecarrot)
- [YouTube](http://www.youtube.com/leecarrot)
- [FriendFeed](http://friendfeed.com/leecarrot)
- [GitHub](http://github.com/rosebery)

=--

About this site
===============
The text files are written using the editor [Gedit][gedit] in the format called [Markdown][md]. These are transformed into HTML by [Maruku][mk]. Based on the clean and beautiful template design by [Mark Reid][mr], the whole process is automated by [Jekyll][jk] to produce a site hosted on my [Github page][rb]. 

[rb]: http://github.com/rosebery/rosebery.github.com
[md]: http://daringfireball.net/projects/markdown/
[mk]: http://maruku.rubyforge.org/
[gedit]: http://projects.gnome.org/gedit/
[jk]: http://jekyllrb.com/
[mr]: http://mark.reid.name/

