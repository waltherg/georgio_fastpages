---
keywords: fastai
description: "In this article I explore basic causal inference, how it differs from machine learning, and how it presents a path forward for robust decision-making in data-driven companies. Here, the ongoing coronavirus / COVID-19 pandemic provides an unfortunate but intriguing challenge to established machine learning applications in industry and enterprises that further rationalizes the need for causal inference methodologies."
title: "Causal inference for robust decision-making in data-driven companies"
published: false
toc: true
branch: master
badges: true
comments: true
categories: [causal inference, data-driven company]
nb_path: _notebooks/2020-05-02-Causal_inference_for_robust_decision-making_in_data-driven_companies.ipynb
layout: notebook
---

<!--
#################################################
### THIS FILE WAS AUTOGENERATED! DO NOT EDIT! ###
#################################################
# file to edit: _notebooks/2020-05-02-Causal_inference_for_robust_decision-making_in_data-driven_companies.ipynb
-->

<div class="container" id="notebook-container">
        
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h1 id="The-data-driven-company">The data-driven company<a class="anchor-link" href="#The-data-driven-company"> </a></h1>
</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h1 id="Machine-learning-for-decision-making">Machine learning for decision-making<a class="anchor-link" href="#Machine-learning-for-decision-making"> </a></h1>
</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h1 id="Issues-with-machine-learning-as-sole-decision-making-tool">Issues with machine learning as sole decision-making tool<a class="anchor-link" href="#Issues-with-machine-learning-as-sole-decision-making-tool"> </a></h1><p>As we have seen, machine learning provides the means to learn relationships from and make decisions
based on data samples.
Of note here is that machine learning does not require us to have an understanding of the causal relationships
underlying our data sample.</p>
<p>This is both a blessing and a curse: Oftentimes it can be straightforward to build machine learning algorithms, such as classification and regression, that produce predictions based on patterns in our data that may be so complex that a human would never uncover them.
However, machine learning algorithms can only uncover and predict patterns that are present in our sample data.</p>
<p>Likely none of the data collected after the 1930s, <a href="https://www.forbes.com/sites/petercohan/2020/04/06/how-covid-19-crunch-compares-to-spanish-flu-great-depression">following the Spanish Flu and the Great Depression</a>, reflect patterns found in sample data since the onset of the global coronavirus pandemic.</p>
<p>Hence, predictions based solely on sample data and produced and entirely with machine learning algorithms will likely be off.</p>
<p>This of course depends on the context and specific problem we attempt to tackle with machine learning:
A machine learning classifier that distinguished traffic signs to help autonomous cars make sensible decisions is not likely to be impacted by the ongoing pandemic - while algorithms that predict market indicators, customer behavior, product demand, or supply chain behavior are probbly heavily impacted.</p>
<p>So what do we need to really leverage machine learning and our vast amounts of data?</p>
<p>We need a clear understanding of the cause-effect relationships underlying the processes and systems that produce our data and we need to enhance our machine learning algorithms with that understanding.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h1 id="Causal-inference">Causal inference<a class="anchor-link" href="#Causal-inference"> </a></h1>
</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h1 id="Causal-inference-for-decision-making">Causal inference for decision-making<a class="anchor-link" href="#Causal-inference-for-decision-making"> </a></h1>
</div>
</div>
</div>
</div>
 
