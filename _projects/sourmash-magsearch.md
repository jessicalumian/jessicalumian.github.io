---
layout: page
title: Biogeography with sourmash MAGsearch
description: Using large-scale k-mer searching to find genomes of interest in public metagenomes
img: assets/img/MAGsearch_map.png
importance: 2
category: research
---

After investigating the metabolic potential of *Phormidium pseudopriestleyi* and finding myself stuck at home during
covid-19 lockdowns, I needed to find a new direction to finish my dissertation.

My lab had sequencing of microbial mats from Lake Vanda, another ice-covered lake in the McMurdo Dry Valleys, so I decided to
obtain additional genomes from this data.

The microbial mat data was assembled into metagenomes and then binned. The best quality bins were recovered as metagenome-assembled genomes
(MAGs). From this work, I generated four new MAGs: a *Leptolyngbya*, *Microcoleus*, *Neosynechococcus*, and *Pseudanabaena*.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/lakes_MAGs.png" title="Map of lakes and novel MAGs" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    A map of the five novel cyanobacteria MAGs from my dissertation.
</div>

These genomes were generated by assembling metagenomes, creating bins, and refining bins of interest. The statistics for these bins are below.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/MAG_stats.png" title="Table of MAGs stats" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    These statistics were generated from QUAST.
</div>

I analyzed photosynthesis and circadian rhythm gene content and compared this to the other polar cyanobacteria genomes (there were only 5 available when I 
was doing this work!).

The really exciting part comes through a collaboration with Luiz Irber, Tessa Pierce-Ward, and Titus Brown at UC Davis. Using a novel bioinformatics 
search technique, we were able to search my MAGs in ~500,000 public metagenomes on the NCBI Sequence Read Archive. These metagenomes come from all over 
the globe, so we were able to identify new environments where these organisms are located.

Biogeography is the study of where organisms are located. Most bacteria biogeography studies are based on the 16S gene, but sourmash MAGsearch allows
us to use the whole genome as a query, which is pretty powerful! This technique searches through metagenomes, which were previously unsearchable because
of how long it would take to search for a genome through 500,000 metagenomes.   

Briefly, this process creates a specific signature of a genome. This signature is searched against the signatures of all metagenomes in the NCBI Sequence
Read Archive. Results are returned based on containment.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/MAGsearch_workflow.png" title="Table of MAGs stats" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    A genome of interest can be used as a search query against a massive amount of data with sourmash MAGsearch.
</div>

The workflow above shows a containment value of 20% for a metagenome of a lagoon in France. This means that 20% of the k-mers in my Antarctic cyanobacteria
genome were found in a lagoon in France!

More details about this process can be found at the following blog posts: [https://blog.luizirber.org/2020/07/24/mag-results/](https://blog.luizirber.org/2020/07/24/mag-results/) 
and [http://ivory.idyll.org/blog/2021-MAGsearch.html](http://ivory.idyll.org/blog/2021-MAGsearch.html).

My results showed me data from around the globe that shared genome content with Antarctic cyanobacteria, and there were some pretty exciting results!

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/MAGsearch_map.png" title="Table of MAGs stats" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Global distribution of cyanobacteria above specified containment values..
</div>

The *Microcoleus* was in a wide variety of environmental conditions. *Phormidium pseudopriestleyi* was found in environments with stressful conditions.
The *Pseudanabaena*, *Leptolyngbya*, and *Neosynechococcus* were found only in cold environments at containment values above the threshold.

It has been exciting to discover different types of cold-tolerant cyanobacteria! The *Microcoleus* can grow in a variety of conditions while 
*Phormidium pseudopriestleyi* seems to thrive in locations that are too stressful for many other organisms.

The details of this work has been written up in my dissertation, and will be in a paper or preprint soon.
