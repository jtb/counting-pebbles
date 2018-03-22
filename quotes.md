---
layout: page
title: Ancient Quotations

quotes:
  - source: Lysias 445 BC – c. 380 BC
    info: something something something
    english: |
      the office furniture of a banker consisted of
      a table and an abacus.
    greek: hi!

---

This page contains a list of quotations about pebbles and counting boards, arranged roughly in chronological order. They offer glimpses into how the ancient Greeks used these counting boards in their daily lives.

<hr class="bigHr">

{% for quote in page.quotes %}
{{quote.source}}

{{quote.info}}
> {{quote.english}}
{% if quote.greek %}
> {{quote.greek}}
{% endif %}

<hr class="bigHr">
{% endfor %}

for quote in page.quotes
include book.html quote=quote 
endfor

{% for book in site.data.bib.books %}
<p>
{% assign thebook = book[1] %}
{% include book.html cite=thebook %}
</p>
{% endfor %}


({{site.data.bib.books.menninger.short}}, p. 93)
<p>
{% include book.html cite=site.data.bib.books.menninger %}
</p>
<p>
{% include book.html cite=site.data.bib.books.scharlig %}
</p>
<p>
{% include journal.html cite=site.data.bib.journals.teriele %}
</p>



Herodotus was a Greek historian who lived in the fifth century BC (c. 484 - c. 425 BC). His work *The Histories* is considered the founding work of history in Western literature. Book II discusses Egypt.
> Finally in the writing of characters and reckoning with pebbles, while the Hellenes carry the hand from the left to the right, the Egyptians do this from the right to the left; and doing so they say that they do it themselves rightwise and the Hellenes leftwise.
>
> * An Account of Egypt, The Histories, c. 440 BC, Book II 36:4 by Herodotus

<hr class="bigHr">

> the office furniture of a banker consisted of a table and an abacus.
>
> * Lysias 445 BC – c. 380 BC

<hr class="bigHr">

*The Wasps* is the fourth in chronological order of the eleven surviving plays by Aristophanes, the master of an ancient genre of drama called 'Old Comedy'. It was produced at the Lenaia festival in 422 BC, a time when Athens was enjoying a brief respite from the Peloponnesian War following a one-year truce with Sparta. The following are two quotations from this work which mention pebbles for counting.

> then carry me hence, and may thy breath hurl me into some strong, hot marinade or turn me into one of the stones on which the votes are counted.
>
> * The Wasps, c. 422 BC, Line 330, by Aristophanes

> Listen to me, dear little father, unruffle that frowning brow and reckon, you can do so without trouble, not with pebbles, but on your fingers, what is the sum-total of the tribute paid by the allied towns; besides this we have the direct imposts, a mass of percentage dues, the fees of the courts of justice, the produce from the mines, the markets, the harbours, the public lands and the confiscations. All these together amount to nearly two thousand talents. Take from this sum the annual pay of the dicasts; they number six thousand, and there have never been more in this town; so therefore it is one hundred and fifty talents that come to you.
>
> * The Wasps, c. 422 BC, Line 655, by Aristophanes

<hr class="bigHr">

Demosthenes (384 - 322 BC) was a Greek statesman and orator of ancient Athens.

> I shall prove without difficulty that he has no right to ask you to reverse that opinion—not by using counters, for political measures are not to be added up in that fashion, but by reminding you briefly of the several transactions, and appealing to you who hear me as both the witnesses and the auditors of my account. 
>
> * On the Crown XVIII, 229, 330 BC, by Demosthenes

<hr class="bigHr">

The *Constitution of the Athenians* is a work by Aristotle or one of his students. It describes the political system of ancient Athens.

> When all the jurors have voted, the attendants take the urn containing the effective votes and discharge them on to a reckoning board having as many cavities as there are ballot balls, so that the effective votes, whether pierced or solid, may be plainly displayed and easily counted. Then the officials assigned to the taking of the votes tell them off on the board, the solid in one place and the pierced in another, and the crier announces the numbers of the votes, the pierced ballots being for the prosecutor and the solid for the defendant. Whichever has the majority is victorious; but if the votes are equal the verdict is for the defendant. Each juror receives two ballots, and uses one to record his vote, and throws the other away. 
>
> * Constitution of the Athenians (330 - 322 BC) Part 69

<hr class="bigHr">

Polybius (c. 200 – c. 118 BC) was a Greek historian of the Hellenistic period noted for his work *The Histories*, which covered the period of 264–146 BC in detail. This delightful metaphor gives evidence that the pebbles on a counting board represented different values depending on the position they were placed. 

> All men are subject to be elevated and again depressed by the most fleeting events but this is particularly the case with those who frequent the palaces of kings. They are like the stones upon abaci, which according to the pleasure of the calculator are at one time of the value of a small copper coin and immediately afterwards are worth a talent of gold. Thus courtiers at the monarch's nod may suddenly become either happy or miserable.
>
> * The Histories (c. 200 – c. 118 BC) Book V 26:13-14, by Polybius

<hr class="bigHr">

Persius (4 December 34, in Volterra – 24 November 62) was a Roman poet and satirist of Etruscan origin. The slab probably refers to a marble abacus, and the cones drawn in the sand probably refers to the figures drawn in sand by geometers such as Archimedes.

> nor the man who has the wit to laugh at the figures on the slab and the cones drawn in sand
>
> * The Satires of A. Persius Flaccus (4 AD - 24 AD)

<hr class="bigHr">

Diogenes Laërtius (c. 3rd century AD) was a biographer of the Greek philosphers. In the below quotation, Diogenes discusses Solon (c. 638 - 558 BC), an Athenian stateman born on the island of Salamis. This quote is similar to the one attributed by Polybius.

> He used to say that those who had influence with tyrants were like the pebbles employed in calculations; for, as each of the pebbles represented now a large and now a small number, so the tyrants would treat each one of those about them at one time as great and famous, at another as of no account.
>
> * Diogenes Laërtius 3rd century AD, Lives of Eminent Philosophers  chapter 2 solon (archon 594 B.C.) 59 

<hr class="bigHr">

The Deipnosophistae is an early 3rd-century AD Greek work by the Greco-Egyptian author Athenaeus of Naucratis. Some references to counting boards in this work are attributed to the 3rd century BC Greek comic poet Alexis. 

> Nevertheless, I mean to sit down here and reckon the cost of my menu, to plan what I must get first, and how I must season each dish.
>
>  * From *The Love-lorn Lass* by Alexis as written in Deipnosophistae by Athenaeus, 117 C-E

> Bring a counting-board and counters.
>  * From *The Man with a Cataract* by Alexis as written in Deipnosophistae by Athenaeus, 117 C-E 

<hr class="bigHr">
