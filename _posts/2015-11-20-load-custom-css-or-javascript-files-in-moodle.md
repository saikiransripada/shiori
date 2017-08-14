---
layout: post
title: Load custom CSS or JavaScript files in Moodle
date: 2015-11-20 10:28:48
tags: moodle
categories: 'blog'
---

<p>To include a CSS file in Moodle:</p>

<pre><code class="language-php">$PAGE-&gt;requires-&gt;css(new moodle_url(/path/to/file.css));</code></pre>

<p>To include a JavaScript file in Moodle:</p>

<pre><code class="language-php">$PAGE-&gt;requires-&gt;js(new moodle_url(/path/to/file.js));</code></pre>

<p>Provide the relative path to the file (excluding document root).</p>

<p>When writing a plugin, place CSS in a file called <code class="language-markdown">styles.css</code> in the base directory of your plugin <code class="language-markdown">/plugin/styles.css</code>. Moodle will automatically load the file for you.</p>