---
layout: post
title:  "Emoji - Planet Jekyll Plugin of the Month - Add Thumbs Up (+1), Smileys n More to Your Pages"
---


Welcome back. 
The Planet Jekyll Plugin of the Month series presents a new addon for your (static) web pages
every month.



## What's the `jemoji` gem?

Let's thank
Ben Balter, Parker Moore and friends who have created the `jemoji` gem 
that lets you add 500+ emojis, that is, similey, thumbs ups (+1s) and more to your pages
using shortcodes.


To spice up your plain text use "shortcodes" that will get (auto-)converted to mini inline pictures. 
Example:

```
I give the jemoji plugin two :+1:!
```

resulting in:

I give the jemoji plugin two :+1:!


## How are you feeling today?

To add a "classic" similey use any of the 20+ shortcodes. Example:

:smile: `:smile:`
:laughing: `:laughing:`
:blush: `:blush:`
:smiley: `:smiley:`
:relaxed: `:relaxed:`
:smirk: `:smirk:`
:heart_eyes: `:heart_eyes:`
:kissing_heart: `:kissing_heart:`
:kissing_closed_eyes: `:kissing_closed_eyes:`
:flushed: `:flushed:`
:relieved: `:relieved:`
:satisfied: `:satisfied:`
:grin: `:grin:`
:wink: `:wink:`
:stuck_out_tongue_winking_eye: `:stuck_out_tongue_winking_eye:`
:stuck_out_tongue_closed_eyes: `:stuck_out_tongue_closed_eyes:`
:grinning: `:grinning:`
:kissing: `:kissing:`
:kissing_smiling_eyes: `:kissing_smiling_eyes:`
:stuck_out_tongue: `:stuck_out_tongue:`
:sleeping: `:sleeping:`
:worried: `:worried:`
:frowning: `:frowning:`
:anguished: `:anguished:`
:open_mouth: `:open_mouth:`
:grimacing: `:grimacing:`
:confused: `:confused:`
:hushed: `:hushed:`
:expressionless: `:expressionless:`
:unamused: `:unamused:`
:sweat_smile: `:sweat_smile:`
:sweat: `:sweat:`
:disappointed_relieved: `:disappointed_relieved:`
:weary: `:weary:`
:pensive: `:pensive:`
:disappointed: `:disappointed:`
:confounded: `:confounded:`
:fearful: `:fearful:`
:cold_sweat: `:cold_sweat:`
:persevere: `:persevere:`
:cry: `:cry:`
:sob: `:sob:`
:joy: `:joy:`
:astonished: `:astonished:`
:scream: `:scream:`
:tired_face: `:tired_face:`
:angry: `:angry:`
:rage: `:rage:`
:triumph: `:triumph:`
:sleepy: `:sleepy:`
:yum: `:yum:`
:mask: `:mask:`
:sunglasses: `:sunglasses:`
:dizzy_face: `:dizzy_face:`
:imp: `:imp:`
:smiling_imp: `:smiling_imp:`
:neutral_face: `:neutral_face:`
:innocent: `:innocent:`
:alien: `:alien:`


## Cats, Cats, Cats

Or add some cats:

:smiley_cat: `:smiley_cat:`
:smile_cat: `:smile_cat:`
:heart_eyes_cat: `:heart_eyes_cat:`
:kissing_cat: `:kissing_cat:`
:smirk_cat: `:smirk_cat:`
:scream_cat: `:scream_cat:`
:crying_cat_face: `:crying_cat_face:`
:joy_cat: `:joy_cat:`
:pouting_cat: `:pouting_cat:`

Or add some roses :rose::rose::rose: or tulips :tulip::tulip::tulip: or
on and on and on. 
See the [Emoji Cheet Sheet](http://planetjekyll.github.io/sandbox-github-pages/emoji-cheat-sheet) 
for more than 500+ shortcodes.


## How does it work?

The emoji plugin runs your text through a filter (that is, `HTML::Pipeline::EmojiFilter`) 
and replaces all known `:shortcodes:`
with images (served from the GitHub.com). Example: 

```
:+1:
```

becomes (in HTML):

```
<img class="emoji" 
     title=":+1:" 
     alt=":+1:"
     src="https://assets-cdn.github.com/images/icons/emoji/unicode/1f44d.png" 
     height="20" width="20" 
     align="absmiddle">
```

resulting in:

:+1:


## Yes, Works with GitHub Pages 

Last but not least - the good news - the `jemoji` gem is an official 
white-listed GitHub Pages plugin. To use it add the following 
to your site's `_config.yml` file:

```
gems:
- jemoji
```

That's it. Happy Publishing with Jekyll.

## Bonus: Can You Crack the Emoji Code?

Easy - 
:see_no_evil:
:hear_no_evil:
:speak_no_evil:

Hard - 
:honeybee:
:honeybee:
:arrows_counterclockwise:
:no_entry_sign:
:honeybee:
:honeybee:
:arrow_right:
:question:

What does it mean?!



## Learn More

- home :: [jekyll/jemoji](https://github.com/jekyll/jemoji)
- gem :: [jemoji](https://rubygems.org/gems/jemoji)
- rdoc :: [jemoji](http://rubydoc.info/gems/jemoji)

