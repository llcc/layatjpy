---
title: "Blog configuration"
date: 2015-06-29
layout: post
categories: [emacs]
---
Blog configuration for blogging the current subtree in org-mode to github.

{% highlight cl %}
(use-package ox-jekyll-subtree
  :load-path "~/.emacs.d/elpa/ox-jekyll-subtree"
  :config
  (progn
    (autoload 'endless/export-to-blog "jekyll-once")
    (setq org-jekyll-use-src-plugin t)
    ;; Obviously, these two need to be changed for your blog.
    (setq endless/blog-base-url "http://llcc.github.io/layatjpy/")
    (setq endless/blog-dir "C:/Users/lzhes/GoogleDrive/Git/layatjpy/")
{% endhighlight %}
