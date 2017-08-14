---
layout: post
title: Stopping and Restarting - Apache HTTP Server
date: 2015-12-04 15:24:29
tags: apache centos linux ubuntu
categories: 'blog'
---

<p>Commands to start, stop, reload or restart an Apache2 web server.</p>

<p><b><span class="underline">Ubuntu</span></b></p>
<pre><code class="language-apacheconf">sudo service apache2 restart</code></pre>

<pre><code class="language-apacheconf">sudo /etc/init.d/apache2 restart</code></pre>

<p><b><span class="underline">Cent OS 6</span></b></p>
<pre><code class="language-apacheconf">sudo service httpd restart</code></pre>

<pre><code class="language-apacheconf">sudo /etc/init.d/httpd restart</code></pre>

<p><b><span class="underline">Cent OS 7</span></b></p>
<pre><code class="language-apacheconf">sudo systemctl restart httpd</code></pre>

<pre><code class="language-apacheconf">sudo /bin/systemctl restart httpd.service</code></pre>

<p>Use <code class="language-markdown">sudo</code> when logged in as a non-root user.</p>

<p>Replace <code class="language-markdown">restart</code> with <code class="language-markdown">start</code>, <code class="language-markdown">stop</code>, <code class="language-markdown">reload</code> or <code class="language-markdown">status</code> to start, stop, reload or check status of Apache web server respectively. Use <code class="language-markdown">reload</code> to restart Apache web server without kicking off your website visitors.</p>