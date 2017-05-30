---
layout: post
title: "CSS: button with round edges"
date: 2017-05-28
---

Sometimes we need to create a button with round edges.

It is simple, if the button has the same width and height and should be totally round. We just can write

{% highlight css %}
.button {
  width: 50px;
  height: 50px;
  border-radius: 50%;
}
{% endhighlight %}

<button class="button" type="button" style="display: block; width: 50px; height: 50px; border-radius: 50%; border: none; background-color: #FF9800; color: white;">Btn</button>

But what if the button should be wide but with round edges?

If we just increase width we get this.

<button class="button" type="button" style="display: block; width: 250px; height: 50px; border-radius: 50%; border: none; background-color: #FF9800; color: white;">Btn</button>

Here css trick comes.

Just give a huge value to button's border-radius.

{% highlight css %}
.button {
  width: 250px;
  height: 50px;
  border-radius: 9999px;
}
{% endhighlight %}

<button class="button" type="button" style="display: block; width: 250px; height: 50px; border-radius: 9999px; border: none; background-color: #FF9800; color: white;">Btn</button>

Hope this helps.
