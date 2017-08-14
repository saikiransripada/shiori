---
layout: post
title: Remove leading and trailing spaces from text in Excel
date: 2016-01-11 15:54:11
tags: excel
categories: 'blog'
---

<p>Remove leading and trailing spaces from text using an excel formula.</p>

<pre><code class="language-markdown">=TRIM(CLEAN(SUBSTITUTE(A1,CHAR(160)," ")))</code></pre>

<p><code class="language-markdown">SUBSTITUTE</code> function replaces all non-breaking spaces with spaces. <code class="language-markdown">CLEAN</code> function removes a range of non-printable characters including line breaks.</p>

<p><code class="language-markdown">TRIM</code> function removes both leading and trailing spaces from text and also removes multiple spaces between words to one space.</p>