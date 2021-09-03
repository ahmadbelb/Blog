---
layout: page
title: "Machine Learning Glossary"
description: "Machine Learning Glossary / Cheat Sheet with a focus on intuition"
header-img: "img/machine-learning-glossary-bg.jpg"
order: 1
mathjax: true
comments:	true
---

Welcome,

This is my **first post ever** :bowtie:, I'd love to get your [feedback](#disqus_thread){:.mdLink}.

<!-- 
What dropdown: start open
 -->

<details open>
  <summary>What</summary>
  
  <div markdown="1">
  I will try to **summarize important terms and concepts of machine learning**. The **focus is on intuition** but there will also be practical and theoretical notes. 
  
  **Target Audience,** this is for you if you:

* Have a decent understanding of a concept but **want more intuition**.
* Are **switching machine learning sub-domains.**
* **Knew a term, but want to refresh** your knowledge as it's hard to remember everything (that's me :sweat_smile: ).
* Need to **learn the important concepts in an efficient way**. Students cramming for an exam: that's for you :four_leaf_clover: !
</div>
</details> 
<p></p>

* any text here
{:toc}


<div>
<details>
  <summary>Why</summary>
  
  <div markdown="1">
  Having a bad memory but being (at least considering myself to be :sweat_smile: ) a philomath who loves machine learning, I developed the habit of taking notes, then summarizing and finally making a cheat sheet for every new ML domain I encounter. There are multiple reasons I want to switch to a web-page: 

  <ul>
    <li>Paper is <b>not practical</b> and prone to loss. </li>
    <li>Thinking that someone I don't know (I'm talking about you :raising_hand: ) might read this post <b>makes me write higher quality notes</b> .</li>
    <li>I'm forever grateful to people that spend time on forums and open source projects. <b>I now want to give back to the community</b> (The contribution isn't comparable, but I have to start somewhere :innocent: ).</li>
    <li>Taking notes on a computer is a necessary step for my migration to CS :sweat_smile: .</li>
    <li>As a wise man once said: <blockquote> You do not really understand something unless you can explain it to your grandmother. <cite> - Albert Einstein </cite>
    	   </blockquote> 
    	   My grandma's are awesome :heart: but not really into ML (yet). You have thus been designated "volunteer" to temporarily replace them.</li>
  </ul> 
  </div>
</details>
</div> 

<p>
<details>
  <summary>Notation</summary>

<div markdown="1">
Keeping a uniform notation in machine learning is not easy as many sub-domains use different notations due to historical reasons. I will try using a uniform notation for all the glossary:  

* Lower case letters (a,b,c,...): scalars and functions. 
* Bold capital letters (**A**,**B**,**C** ...): matrices. 
* Bold lower case letters (**a**,**b**,**c** ...): vectors. 
* Capital letters (X,Y,Z...): either a random variable or a number of values an index can take (*e.g.* $k=1 \ldots K$) 
* Superscripts with $(n)$ (*e.g.* $x^{(n)}$) are used to denote one of the $T$ training examples. Superscripts with $(t)$ denote one of the $T$ test examples.
</div>
   
    
  
<div markdown="1">
To make it easier to search the relevant information in the Glossary here is the color coding I will be using:  

<ul style="list-style: none;">
<li class="col-xs-6"> :bulb: <span class="intuition"> Intuition </span> </li>
<li class="col-xs-6"> :wrench: <span class="practice"> Practical </span> </li>
<li class="col-xs-6"> :x: <span class="disadvantage"> Disadvantage </span> </li>
<li class="col-xs-6"> :white_check_mark: <span class="advantage"> Advantage </span> </li>
<li class="col-xs-6"> :school_satchel: <span class="example"> Example </span> </li>
<li class="col-xs-6"> :mag: <span class="note"> Side Notes </span> </li>
<li class="col-xs-6"> :wavy_dash: <span class="compare"> Compare to </span> </li>
<li style="position:relative;left:15px;"> :information_source: <span class="resources"> Resources </span><br /> </li>
</ul> 
</div>
</details>
</p>


**Disclaimer**: 
* This is my **first post ever** :bowtie:, I would love to get your [feedback](#disqus_thread){:.mdLink}.
* I'm bad at spelling: **Apologies in advance** (feel free to correct me).    
* **Check out the [resources](/resources/){:.mdLink}** from where I got most of this information. 
* ML sub-domains overlap **A LOT**. I'll try not to make the separations too artificial. Any suggestions would be appreciated :relaxed: . Note that I separate domains both by *learning style* and by *algorithm similarity*. 
* This is not meant to be a post read in order, but rather used as a "cheat-sheet". Use the [table of content](#markdown-toc){:.mdLink} or `Ctrl+f`.
* Many parts are still missing, come back soon for those.

Enough talking: prepare your popcorn and let's get going :clapper: ! 

## General Machine Learning Concepts
{% include_relative _glossary/concepts.md %}

## Supervised Learning
{% include_relative _glossary/supervised.md %}

## Unsupervised Learning
{% include_relative _glossary/unsupervised.md %}

## Reinforcement Learning
{% include_relative _glossary/RL.md %}

## Partially Supervised Learning
{% include_relative _glossary/partialSupervised.md %}

----
The  previous sections were separated by learning style. I will now separate by algorithm similarity.

----
## Bayesian Methods
{% include_relative _glossary/bayesian.md %}

## Deep Learning
{% include_relative _glossary/DL.md %}

## Graphical Models
{% include_relative _glossary/graphicalModels.md %}

----
The  previous sections were separated by learning style and algorithm similarity. I will now focus on the application.

----

## Automatic Speech Recognition
{% include_relative _glossary/speech.md %}

## Computer Vision
{% include_relative _glossary/cv.md %}

## Natural Language Processing
{% include_relative _glossary/NLP.md %}

## Time Series
{% include_relative _glossary/timeSeries.md %}

---
The following sections are not strictly speaking part of Machine Learning. They are nevertheless very related and important.

---

## Optimization
{% include_relative _glossary/optimization.md %}

## Computational Neuroscience
{% include_relative _glossary/neuroscience.md %}

Unfortunately here ends today's journey together. But don't be too disappointed, I'm only getting started. I still have a tuns of notes eagerly waiting to get upgraded, and I don't intend to stop learning yet :sweat_smile:. 

PS: Any reaction/suggestions would be very appreciated: just drop a comment below or click on the :heart: .

See you soon !



