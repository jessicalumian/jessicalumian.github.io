---
layout: page
title: Sulfide-tolerant Cyanobacteria
description: The metabolic potential of Phormidium pseudopriestleyi, a sulfide-tolerant Antarctic cyanobacteria
img: assets/img/phormidium.jpg
importance: 1
category: research
---

The McMurdo Dry Valleys contain perennially ice-covered lakes that are home to microbial mats consisting of cyanobacteria 
and other microscopic organisms. 

These cyanobacteria face many stresses! After surviving a freeze drying trip through the  atmosphere to get to Antarctica, 
cold temperatures and limited light availability throughout the year can hamper growth.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/fryxell_map.jpg" title="Map of Lake Fryxell" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Maps from Sumner et al, 2015. <a href="https://doi.org/10.1130/G36966.1">doi.org/10.1130/G36966.1</a>
</div>

Lake Fryxell is home to *Phormidium pseudopriestleyi*, a cyanobacteria that grows in cold, low light, and sulfidic conditions.
This is impressive because:

- Cold temperatures slow biochemical processes. 
- Light is required for photosynthesis. 
- Sulfide normally inhibits photosynthesis. 

*Phormidium pseudopriestleyi* is the dominant cyanobacteria that grows in sulfidic parts of the water. Understanding how this organism
tolerates sulfide would broaden the understanding of sulfide stress in cyanobacteria.

To better study this mechanism, *Phormidium pseudopriestleyi* was cultured from a frozen chunk of Lake Fryxell microbial mat and sequenced. 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/mat_chunk.jpg" title="Chunk of microbial mat" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    A frozen chunk of microbial mat from Lake Fryxell. The dark green bits are Phormidium pseudopriestleyi!
</div>

It took some time to figure out how to best grow this organism in the lab. Eventually, Green filaments were pulled from the mat chunk and grown in BG11 agar plates.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/phormidium.jpg" title="Phormidium in plate" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The filamentous cells can spread out within the well or get tangled.
</div>

Under the microscope, the cells look like long filaments.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/phormidium_microscope.jpg" title="Phormidium in underscope" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    This image is taken at 30X magnification.
</div>

After sequencing the organism, I generated a genome and analyzed its metabolic potential. 

I had metagenomic sequencing from a microbial mat sample and deeper sequencing from a lab culture. I created a Snakemake pipeline to generate a genome
from the coassembly. The code for this process can be found at [https://github.com/jessicalumian/fryxell-phormidium](https://github.com/jessicalumian/fryxell-phormidium).

Based on gene content, there are three mechanisms
that could help *Phormidium pseudopriestleyi* tolerate sulfide. I created the figure below to illustrate how sulfide inhibits oxygenic photosynthesis
and the ways sulfide may be oxidized.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/phormidium_sulfide_figure.png" title="Diagram of sulfide tolerance mechanisms" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Sulfide tolerance mechanisms figure from Lumian et al., 2021. <a href="https://doi.org/10.3390/genes12030426">doi.org/10.3390/genes120304261</a>.
</div>

I determined that the sulfide could be depleted by anoxygenic photosynthesis, abiotic sulfide oxidation, or a combination of the two. Low light in
the environment may also play a role, and of course we can't discount the potential influence of nearby organisms!

You can read about the whole story in the paper here at [Lumian, et al. 2021](https://doi.org/10.3390/genes12030426).

The next step to figuring out this mechanism would be to replicate the sulfidic conditions of Lake Fryxell in the lab and measure the response of 
*Phormidium pseudopriestleyi*. I planned these experiments, but they were unfortunately canceled due to covid-related lab shutdowns.

Instead, I generated more Antarctic cyanobacteria genomes and conducted a biogeography study with them. This turned out to be pretty exciting, and you can read more 
about that at its project page.

