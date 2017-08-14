---
title: List all views in a MySQL database
date: 2016-03-17 16:23:25
categories: [Database, MySQL]
---

<p>SQL command to display all views in a database.</p>

<pre><code class="language-sql">SHOW FULL TABLES WHERE TABLE_TYPE = 'VIEW';</code></pre>

OR

<pre><code class="language-sql">SHOW FULL TABLES IN &lt;database_name&gt; WHERE TABLE_TYPE = 'VIEW';</code></pre>

<p>You must have a database selected when using the first one. Use latter without selecting a database.</p>