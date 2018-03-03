---
layout: article
title:  "Today I Learned #1 - Validate JSON Files using CLI"
date:   2018-03-03 16:38:47 +0800
group: "blog"
comments: true
---
Install `jsonlint`
{% highlight shell %}
npm install jsonlint -g
{% endhighlight %}

Navigate to the directory and validate all `.json` files in that directory.
{% highlight shell %}
find . -name \*.json  | xargs -I {} jsonlint -q {}
{% endhighlight %}

This will output the syntax that is causing an error in my case it was `<<<<< HEAD` that I missed from rebasing.

Next thing we do is find the file.

Install `ack-grep`
{% highlight shell %}
sudo apt-get install ack-grep
{% endhighlight %}

Then run
{% highlight shell %}
`ack-grep '<<<<< HEAD'`
{% endhighlight %}

This will output the directory of the culprit file.

## Things that can be improved on
<hr class='divider--fade' />

Print out the direct and the file name in the `jsonlint` script. I will update the script if I will be able to find out how or if someone can point it out.

## Sources
<hr class='divider--fade' />

- [Detect invalid JSON files in directory tree](https://superuser.com/a/699897/678407)
- [how to find a word in text files from a directory](https://askubuntu.com/a/462279/634714)
