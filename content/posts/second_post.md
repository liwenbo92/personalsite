Title: Second Post
Date: 2018-11-18
Status: published
Category: example posts
Slug: second-post
Authors: Wenbo Li
Series: example-posts
Series_index: 2
Summary: This is the second post of a series of posts. It will show how to embeded youtube video using pelican.

This is the second post of a series of posts. It shows an embedded youtube video. 

{% youtube 3-bwXhts8Zg [640] [390] %}

To do so I followed [the tutorial](https://pythonforundergradengineers.com/how-i-built-this-site-4.html). Since some of the materials there are out of date, so I explain a little bit in the following. You could use the plugin `liquid_tags.youtube` in `pelicanconf.py` file.

```py
#pelicanconf.py

PLUGINS = [
	'liquid_tags.youtube']
```

And then include the following line in your post `second_post.md`.

```md
{% youtube Qq-5frjUfK0 [640] [390] %}
```

Notice here the difference between the one in [the tutorial](https://pythonforundergradengineers.com/how-i-built-this-site-4.html) and the above is that I only write the video id for the youtube video instead of the full https address.

