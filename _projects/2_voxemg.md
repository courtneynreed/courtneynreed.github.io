---
layout: page
title: voxemg<br>(v3.1)
description: a PCB pre-amplifier for vocal sEMG signals, designed for the small laryngeal muscles
img: assets/img/proj_preview/voxemg.jpg
importance: 1
category: designs
related_publications: Reed_NIME20_VocalsEMG, Reed_TEI21_sEMGPerformance, Reed_AHs22_SingingKnit
---

{% if site.data.repository-voxemg.github_repos %}
<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for repo in site.data.repository-voxemg.github_repos %}
    {% include repository/repo.html repository=repo %}
  {% endfor %}
</div>
{% endif %}

<br>
[The VoxEMG is fully open source and all schematics, CAD files, and instruction for implementation can be found on Github.](https://github.com/courtcourtaney/voxEMG)


<div class="row">
    <div class="col-sm mt-4 mt-md-0">
        {% include figure.html path="assets/img/proj-voxemg/voxemg.png" title="" class="img-fluid rounded" %}
    </div>
    <div class="col-sm mt-2 mt-md-0">
        {% include figure.html path="assets/img/proj-voxemg/VoxEMG-bela.png" title="" class="img-fluid rounded" %}
    </div>
    <div class="col-sm mt-2 mt-md-0">
        {% include figure.html path="assets/img/proj-voxemg/VoxEMG-bela-2.png" title="" class="img-fluid rounded" %}
    </div>
</div>
<div class="caption">
    PCB versions of the VoxEMG. The v3.1 eTextile Configuration (left) features castellated inputs for conductive thread input and loops for textile integration. The v3.1.2 Bela Mini Capelet (middle, right) slots directly into the A0 and A1 analogue inputs, power, and ground from the Bela Mini.
</div>

## about

The VoxEMG circuit is an extension of the open-source [EMG Circuit v7.1 (Advancer Technologies)](advancertechnologies.com/p/muscle-sensor-emg-circuitkit-bronze.html), from which other EMG platforms such as the Myoware are derived. VoxEMG is specifically aimed to detect activation of the extrinsic laryngeal muscles in both vocalised and subvocalised singing. High-precision and trimmable resistors are used to ensure noise reduction and the circuit is flexible to be used with different types of electrodes for desired implementation. The EMG signals can then be used in a variety of manners, for instance to relay feedback about the singer's movements during practice. <br>

There are currently two open-source versions of the VoxEMG available on GitHub. The PCB configurations use the same circuit implemented in different PCB setups:
* [v3.1 - eTextile Configuration](https://github.com/courtcourtaney/voxEMG?tab=readme-ov-file#v31---etextile-configuration) - designed for textile integrations and conductive thread input
* [v3.1.2 - Bela Mini Capelet](https://github.com/courtcourtaney/voxEMG?tab=readme-ov-file#v312---bela-mini-capelet) - designed for direct plug-and-play with the Bela Mini

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/proj-voxemg/workflow.png" title="" class="img-fluid rounded" %}
    </div>
</div>
<div class="caption">
    The VoxEMG signal flow diagram for each muscle input and output.
</div>

## related publications:
