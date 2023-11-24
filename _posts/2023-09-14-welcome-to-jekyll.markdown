---
layout: post
title:  "Let's dig!"
date:   2023-09-14 10:02:50 +0300
categories: jekyll update
---
One of my favorite ruby hash method is `dig` method.

As documentation said it `Extracts the nested value specified by the sequence of key objects by calling dig at each step, returning nil if any intermediate step is nil.`

I like it because it's syntax. When there is a nested hash it is obvious that we want to dig some value :)

{% highlight ruby %}
hash = {a: '1', b: {c:'2', d: '3'}}

print hash[:b][:c]
#=> prints '2' to STDOUT.

print hash.dig(:b, :c)
#=> prints '2' to STDOUT.

{% endhighlight %}

Check out the [Ruby documentation][ruby-docs] for more info.

[ruby-docs]: https://apidock.com/ruby/Hash/dig
