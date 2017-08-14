---
layout: post
title: Get username from email address in Excel
date: 2016-01-05 13:54:34
tags: excel
categories: 'blog'
---

<p>Extract username from an email address using an excel formula.</p>

<pre><code class="language-markdown">=LEFT(A1,FIND("@",A1) - 1)</code></pre>

OR

<pre><code class="language-markdown">=LEFT(A1,SEARCH("@",A1) - 1)</code></pre>

<p><code class="language-markdown">FIND</code> is case-sensitive, <code class="language-markdown">SEARCH</code> isn't. It makes no difference for punctuation searches. Replace <code class="language-markdown">A1</code> with the cell that contains the email address.</p>