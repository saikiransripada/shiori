---
layout: post
title: Font from origin has been blocked from loading by Cross-Origin Resource Sharing policy
date: 2016-02-19 11:24:09
tags: apache
categories: 'blog'
---

<p><p>Custom web fonts via CDN requires custom CORS (Cross-Origin Resource Sharing) configuration to display fonts properly.</p>

<p>Add the below rule to your .htaccess</p>

<pre><code class="language-apacheconf"># Allow access from all domains for webfonts.
&lt;IfModule mod_headers.c&gt;
  &lt;FilesMatch "\.(ttf|ttc|otf|eot|woff|font.css|css)$"&gt;
    Header add Access-Control-Allow-Origin "*"
  &lt;/FilesMatch&gt;
&lt;/IfModule&gt;
</code></pre>

<p>Using a wildcard is potentially insecure as it opens the domain to JavaScript access from any domain. Instead of using a wildcard, you can allow your domain or subdomain.</p>

<pre><code class="language-apacheconf">Header add Access-Control-Allow-Origin "your-domain.com"</code></pre>

<p>When <code class="language-markdown">add</code> is used, the response header is added to the existing set of headers even if this header already exists; Whereas with <code class="language-markdown">set</code> the response header is set, replacing any previous header with this name.</p>

<p>Source:</p>
<ol><li><a href="http://stackoverflow.com/a/26521650">http://stackoverflow.com/a/26521650</a><br></li><li><a href="http://stackoverflow.com/a/28236969">http://stackoverflow.com/a/28236969</a><br></li></ol></p>