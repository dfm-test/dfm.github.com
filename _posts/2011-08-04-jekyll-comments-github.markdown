---
    layout: post
    title: Jekyll blog comments for nerds
    excerpt: How to use GitHub forks for commenting on Jekyll blogs.
---

_This has been temporarily disabled while I update the layout. Sorry!_

I like GitHub a lot. That's why I host many of my projects on it and even my
blog.  In that spirit, I decided to code up a (mildly convoluted) way of
posting comments on my [static Jekyll blog](https://github.com/mojombo/jekyll)
using GitHub forks.

If you click on the "post a comment" link, below, it will -- after checking
with you first -- fork the Textile source for this page using your GitHub
account and then let you edit it. After you add your comment, you can simply
submit it as a pull request.

## How to add a comment

At the very end of the Textile document, you'll find a little snippet of
JavaScript that looks something like:

{% highlight javascript %}
var comments = [
/* begin template --- copy these lines then use any valid html
                                            in your comment */
    {'github_user': 'template',
            'date': new Date(2011,8,3),
        'comment': "This is an example comment.<br />\
                    Don't forget to escape your newlines!"},
/* end template */
]
{% endhighlight %}

Then,

1. copy lines 4-7 and insert them after `@/* end template */@`,
2. fill in your GitHub username, the date and your comment in the appropriate
   fields,
3. and finally, submit the pull request.

It's not elegant but it _is_ a novelty! Let me know what you think in the
comments section below.

## Comments

* github-username - January 1, 2012 - Your comment...
* dfm - August 5, 2011 - This is what a comment looks like!
  Let me know what you think...
* jonathansick - August 6, 2011 - If spam-bots start figuring out how to
  make comments... that'll be the day...
* jakemannix - November 14, 2011 - Given the relative difficulty of
  making comments like this, I'm pretty sure that this will be the most
  spam-free blog in the blogosphere.  It may also be the most
  _comment_-free blog as well, but that's O.K.!  Nice work.

