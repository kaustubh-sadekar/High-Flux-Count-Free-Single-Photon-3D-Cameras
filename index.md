---
layout: default
---

# High-Flux Count-Free Single-Photon 3D Cameras
<a href="https://kaustubh-sadekar.github.io/" target="_blank">Kaustubh Sadekar</a>, <a href="https://www.vivekgoyal.org/" target="_blank">Vivek K Goyal</a>, <a href="https://web.cecs.pdx.edu/~maier/" target="_blank">David Maier</a>, <a href="https://web.cecs.pdx.edu/~ingle2/" target="_blank">Atul Ingle</a>

<a href=" " target="_blank">Arxiv</a> link / <a href=" " target="_blank">ICCP</a> link / <a href="https://github.com/kaustubh-sadekar/High-Flux-Count-Free-Single-Photon-3D-Cameras/" target="_blank">Code</a> (Coming Soon).

# Abstract

Single-photon cameras based on single-photon avalanche diode (SPAD) technology are gaining popularity for 3D sensing, thanks to their extreme sensitivity and time resolution.
There are two key challenges with single-photon cameras that limit their widespread use: (i) they suffer from non-linear distortions called ``pile-up'' when operated in high-photon-flux conditions, and (ii) they generate a large volume of raw photon data, creating a severe data bottleneck at each sensor pixel.
In this work, we show that while compressive capture techniques successfully mitigate data transfer challenges, they exacerbate the effects of dead-time distortion because they fail to retain sufficient information about the photon detection history to allow post-processing pile-up correction via existing methods.
We propose a new computational-imaging method that combines free-running capture with an analysis-by-synthesis software pipeline to mitigate pile-up distortions.
Our results with hardware emulations and full-scene and single-pixel simulations show that our method can reliably capture scene distance and reflectance over a wide range of illumination conditions.
Our work will enable high-resolution SPAD cameras that are severely bandwidth-constrained to operate in real-world high-flux scenarios.


<div style="text-align:center">
    <img src="{{ site.baseurl }}/media/FullScene_iTof2dToF_Results_16bin_with_transients.png" />
</div>

> **Results on 3D scenes with multi-path interference from iToF2dToF dataset.** We compare our EDH-based AbS method with standard baselines that use Equi Width Histograms (EWH) and a histogramless approach. Considering resource-constrained scenarios, we keep the number of EWH bins and EDH bins equal for comparison. Quantitative results: mean error (ME, in meters), standard deviation (SD, in meters), and 1\% inlier rate (1\%in)—are reported beneath each result. As shown, our proposed method significantly reduces distance artifacts and outperforms the baselines. Additionally, we show recovered transients for some selected pixels from each scene, demonstrating how, despite the presence of multi-path interference, our method is able to converge closer to the largest peak in most scenarios.


# Citation
To be added

# Acknowledgments
This work was supported in part by NSF ECCS 2138471 and the Portland State University Venture Development Fund. We thank Keylan Petty for assistance with initial exploratory simulations on the effect of dead-time on ED histogrammers.

# Contact
Feel free to contact <a href="https://kaustubh-sadekar.github.io/" target="_blank">Kaustubh Sadekar</a> for any further discussion about our work.
