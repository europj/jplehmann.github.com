---
layout: post
title: "In the Beginning: There was a sandbox"
date: 2013-03-15 18:38
comments: true
categories: [Dart, Cool, Test]
---

Please allow myself to introduce... myself.

<!-- more -->

This page is a *sandbox* for me to experience with features of the **Octopress** platform.

Octopress is built atop [Jekyll], the static site generator powering GitHub pages. It and utilizes by default the [RDiscount] markdown engine plus [Liquid] templating. RDiscount is based on [standard Markdown][md] by John Gruber. Liquid provides lots of nifty filters and tags.

Markdown is nice for all kinds of basic text decoration. For instance, you can indicate `inline code` with backticks.

#### What you can definitely expect:

* Death
* Taxes
* Lists on my blog

   [Jekyll]: https://github.com/mojombo/jekyll
   [RDiscount]: https://github.com/rtomayko/rdiscount
   [Liquid]: https://github.com/shopify/liquid/wiki/liquid-for-designers
   [md]: http://daringfireball.net/projects/markdown/syntax

Let's start with an adorable kitten.

{% img left http://placekitten.com/320/250 Place Kitten #2 %}

Bacon ipsum dolor sit amet doner salami frankfurter beef pastrami ground round t-bone shank. Pork ham hock salami, strip steak short loin swine biltong hamburger pork loin capicola tongue pig tri-tip frankfurter. Bacon turducken cow chicken jowl shankle. Ball tip beef ribs short loin ham hock boudin pork loin beef shoulder fatback salami cow strip steak kielbasa turducken chicken. Tenderloin tongue ball tip andouille jerky drumstick, brisket cow meatball salami chuck ribeye turkey swine. Leberkas turkey boudin swine spare ribs hamburger meatball.

Then there's the blockquote:

{% blockquote @jplehmann https://twitter.com/jplehmann/status/312615496270884864 %}
In fact, stripping out all the comments before pushing code to master does not make it run any faster.  {% endblockquote %}

Standard snippet for embedding a tweet: 

<blockquote class="twitter-tweet"><p>Detailed list of people who asked for your opinion: ________ ________ ________ ________ ________ ________ ________ ________________</p>&mdash; Grumpy Cat(@ItsTheGrumpyCat) <a href="https://twitter.com/ItsTheGrumpyCat/status/292462511922479104">January 19, 2013</a></blockquote>
<script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

<br>
When you come to the text you want to pull, you embed it. Cow sausage brisket ground round flank sirloin capicola jerky.  Surround your paragraph with the pull quote tags. {% pullquote %}   Turducken pork belly beef cow, pork boudin andouille drumstick tongue bacon. {"Bacon Ipsum is more filling than the rest."}  Chuck beef ribs turducken, kielbasa venison ham hock swine cow sausage brisket ground round flank sirloin capicola jerky.  Ground round shankle rump filet mignon. Brisket pork filet mignon tongue shoulder.  Rump short ribs capicola brisket sausage filet mignon salami corned beef sirloin biltong. Pancetta boudin tri-tip kielbasa bacon.
{% endpullquote %}

Then there were videos.

<iframe width="420" height="315" src="http://www.youtube.com/embed/HQqIQyT-RuM?rel=0&start=48" frameborder="0" allowfullscreen></iframe>

{% comment %}
{% video http://www.youtube.com/watch?v=HQqIQyT-RuM 420 315 %}
{% endcomment %}

<br><br>
Let's turn to code.

    By simply indenting 4 spaces,
    we get a code block, thanks to Markdown.

Codeblock plugin activated via triple-backticks gives us line numbers:
```
$ sudo make me a sandwich
```

With syntax highlighting:
``` python
def something_cool(a, b):
  return a + b
```

Here's one with a url:

``` ruby Discover if a number is prime http://www.noulakaz.net/weblog/2007/03/18/a-regular-expression-to-check-for-prime-numbers/ Source Article
class Fixnum
  def prime?
    ('1' * self) !~ /^1?$|^(11+?)\1+$/
  end
end
```

Inline code blocks here.

{% codeblock Time to be Awesome - awesome.rb %}
puts "Awesome!" unless lame
{% endcodeblock %}

Or another one

{% codeblock Javascript Array Syntax lang:js http://j.mp/pPUUmW MDN Documentation %}
var arr1 = new Array(arrayLength);
var arr2 = new Array(element0, element1, ..., elementN);
{% endcodeblock %}

Here's a gist:

{% gist 996818 %}

Some jsFiddle:

{% jsfiddle ccWP7 %}




