---
layout: page
title: Bibliography
---

<h2 class="greekify">BOOKS</h2>

<ol>
{% assign sorted_books = site.data.bib.books | sort:"short" %}
{% for book in sorted_books %}
<li class="bib" id="{{book.id}}">
<p>
{% include book.html cite=book %}
</p>
</li>
{% endfor %}
</ol>

<h2 class="greekify">JOURNALS</h2>

<ol>
{% assign sorted_journals = site.data.bib.journals | sort:"short" %}
{% for journal in sorted_journals %}
<li class="bib" id="{{journal.id}}">
<p>
{% include journal.html cite=journal %}
</p>
</li>
{% endfor %}
</ol>