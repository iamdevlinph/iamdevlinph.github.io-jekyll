---
layout: article
title:  "Moving to a new domain"
date:   2018-07-11 23:04:30 +0800
updated_date: 2018-07-15 17:19:08 +0800
group: "blog"
comments: true
---
## Update: 15-July-2018

If you are seeing this then it means you are trying to access one my old domain.

I have completely moved to a new domain. You will be redirected automatically in 10 seconds.

If not, you can click <a href="#" id="redirect">here</a>

---

I will be moving to a new domain.

I forgot the 2FA for my godaddy account and removing it is a hassle. So I'll just ditch my current domain and find another one.

I will update this post if I already have a new domain.

Stuff to change when using the new domain :(

* Disqus URL
* Google Webmasters
* Google Analytics
* Set-up URL stuff

<script>
(function () {
  setTimeout(function(){
    var url = new URL(window.location.href);
    var redirect = url.searchParams.get('redirect');
    if (redirect) {
      var newUrl = redirect.replace(/iamdevlinph.me\b/g, 'iamdevlinph.com');
      var redirectAnchor = document.getElementById('redirect');
      redirectAnchor.href  = newUrl;
      window.location.replace(newUrl);
    }
  }, 10000);
})();
</script>
