---
layout: page
title: Bibliography
---

## Books

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

## Journals

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