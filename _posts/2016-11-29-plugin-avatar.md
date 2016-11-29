---
layout: post
title:  "Avatar - Planet Jekyll Plugin of the Month - Add Profile Pics (Speakers, Members, etc.) to Your Pages"
---


Welcome. 
The Planet Jekyll Plugin of the Month series presents a new addon for your (static) web pages
every month.



## What's the `jekyll-avatar` gem?

Let's thank
Ben Balter who has created the `jekyll-avatar` gem 
that lets you add GitHub avatars, 
that is, user profile pics - to your pages.


Use the new `avatar` tag and pass in the user's login. Example:

```
{% raw %}
{% avatar benbalter %}
{% endraw %}
```

will result in:

{% avatar benbalter %}

or in HTML:

```html
<img class="avatar avatar-small" 
     src="https://avatars3.githubusercontent.com/benbalter?v=3&amp;s=40" 
     alt="benbalter" 
     srcset="https://avatars3.githubusercontent.com/benbalter?v=3&amp;s=40 1x, 
             https://avatars3.githubusercontent.com/benbalter?v=3&amp;s=80 2x, 
             https://avatars3.githubusercontent.com/benbalter?v=3&amp;s=120 3x, 
             https://avatars3.githubusercontent.com/benbalter?v=3&amp;s=160 4x" 
     width="40" height="40" />
```


## Big, Bigger, Biggest

Use the size argument to make the avatar bigger. Example:

```
{% raw %}
{% avatar benbalter size=80 %}
{% avatar benbalter size=100 %}
{% avatar benbalter size=150 %}
{% endraw %}
```

will result in:

{% avatar benbalter size=80 %}
{% avatar benbalter size=100 %}
{% avatar benbalter size=150 %}


## All Together 

If you have a list of users e.g. speakers, members, etc. 
use a loop. Example:

```
{% raw %}
{% for member in site.data.members %}
    {% avatar user=member.github size=50 %}
{% endfor %}
{% endraw %}

```

(Source: [viennahtml.github.io/_includes/members.html](https://github.com/viennahtml/viennahtml.github.io/blob/master/_includes/members.html))

resulting in:

{% avatar geraldb size=50 %}
{% avatar dervondenbergen size=50 %}
{% avatar floord size=50 %}
{% avatar karlhorky size=50 %}
{% avatar ramonh size=50 %} 
{% avatar nikgraf size=50 %} 
{% avatar spuz size=50 %} 
{% avatar marfi size=50 %} 
{% avatar haslinger size=50 %} 
and many more ;-)


## Yes, Works with GitHub Pages 

Last but not least - the good news - the `jekyll-avatar` gem is an official 
white-listed GitHub Pages plugin. To use it add the following 
to your site's `_config.yml` file:

```
gems:
- jekyll-avatar
```

That's it. Happy Publishing with Jekyll.

## Bonus: Build the next Meetup.com - Example: Vienna.html (Static) Meetup Site

Why not build your next meetup site with Jekyll?
See the [Vienna.html meetup site](http://viennahtml.github.io/) as a (real-world) live example ;-) - 
[Site Sources](https://github.com/viennahtml/viennahtml.github.io), 
[Members Page](http://viennahtml.github.io/members), 
[Speakers Page](http://viennahtml.github.io/speakers), etc.

## Learn More

- home :: [benbalter/jekyll-avatar](https://github.com/benbalter/jekyll-avatar)
- gem :: [jekyll-avatar](https://rubygems.org/gems/jekyll-avatar)
- rdoc :: [jekyll-avatar](http://rubydoc.info/gems/jekyll-avatar)
