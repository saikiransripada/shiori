---
layout: post
title: Get the file extension in PHP
date: 2015-11-24 17:25:49
tags: php
categories: 'blog'
---

<p><p>A simple function to get the extension of a file. Meet <code class="language-php">pathinfo()</code></p>

<pre><code class="language-php">$extension = pathinfo($filename, PATHINFO_EXTENSION);</code></pre></p>