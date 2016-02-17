---
layout: pub
section: Publications
top: Publications
permalink: /pubs/paper-moderately-stiff-GPU/
title: "Accelerating moderately stiff chemical kinetics in reactive-flow simulations using GPUs"
author: "Kyle E. Niemeyer and Chih-Jen Sung"
date: 2014
journal: "Journal of Computational Physics"
doi: "10.1016/j.jcp.2013.09.025"
arxiv: 1309.2710
supplement:
citation: "Kyle E. Niemeyer and Chih-Jen Sung (2014), Accelerating moderately stiff chemical kinetics in reactive-flow simulations using GPUs, *Journal of Computational Physics*, 256:854--871. doi:10.1016/j.jcp.2013.09.025"
pdf:
---

{{page.title}}
==============

## Abstract

The chemical kinetics ODEs arising from operator-split reactive-flow simulations were solved on GPUs using explicit integration algorithms. Nons- tiff chemical kinetics of a hydrogen oxidation mechanism (9 species and 38 irreversible reactions) were computed using the explicit fifth-order Runge--Kutta--Cash--Karp method, and the GPU-accelerated version performed faster than single- and six-core CPU versions by factors of 126 and 25, respectively, for 524,288 ODEs. Moderately stiff kinetics, represented with mechanisms for hydrogen/carbon-monoxide (13 species and 54 irreversible reactions) and methane (53 species and 634 irreversible reactions) oxidation, were computed using the stabilized explicit second-order Runge--Kutta--Chebyshev (RKC) algorithm. The GPU-based RKC implementation demonstrated an increase in performance of nearly 59 and 10 times, for problem sizes consisting of 262,144 ODEs and larger, than the single- and six-core CPU-based RKC algorithms using the hydrogen/carbon-monoxide mechanism. With the methane mechanism, RKC-GPU performed more than 65 and 11 times faster, for problem sizes consisting of 131,072 ODEs and larger, than the single- and six-core RKC-CPU versions, and up to 57 times faster than the six-core CPU-based implicit VODE algorithm on 65,536 ODEs. In the presence of more severe stiffness, such as ethylene oxidation (111 species and 1566 irreversible reactions), RKC-GPU performed more than 17 times faster than RKC-CPU on six cores for 32,768 ODEs and larger, and at best 4.5 times faster than VODE on six CPU cores for 65,536 ODEs. With a larger time step size, RKC-GPU performed at best 2.5 times slower than six-core VODE for 8192 ODEs and larger. Therefore, the need for developing new strategies for integrating stiff chemistry on GPUs was discussed.

## BibTeX

    @article{Niemeyer:2014jcp,
        Author = {Kyle E Niemeyer and Chih-Jen Sung},
        Title = {Accelerating moderately stiff chemical kinetics in reactive-flow simulations using GPUs},
        Journal = {J. Comput. Phys.},
        Pages = {854--871},
        Volume = {256},
        Year = {2014}
    }