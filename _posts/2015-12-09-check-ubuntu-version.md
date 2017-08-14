---
layout: post
title: Check Ubuntu Version
date: 2015-12-09 18:05:29
tags: linux ubuntu
categories: 'blog'
---

<p>Command to find Ubuntu version.</p>

<pre><code class="language-apacheconf">lsb_release -d</code></pre>

OR

<pre><code class="language-apacheconf">cat /etc/lsb-release</code></pre>

<p>Using options <code class="language-markdown">-c</code>, <code class="language-markdown">-d</code>, <code class="language-markdown">-r</code> displays codename, description (OS name &amp; release number) and release number respectively whereas <code class="language-markdown">-a</code> option displays the information with <code class="language-markdown">-cdr</code> combined.</p>