---
permalink: /
title: "About me"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am currently working as a Tenure Track Assistant Professor at [Science Mathematics and Technology Cluster](https://smt.sutd.edu.sg/) of Singapore University of Technology and Design. 

Previously I was a Research Fellow at [Centre for Quantum Technologies, National University of Singapore](https://www.quantumlah.org/), collaborating with Prof. [Patrick Rebentrost](https://www.quantumlah.org/people/profile/Frank-Patrick). 

I got my PhD degree in July 2022 from [Institute of Theoretical Physics, Chinese Academy of Sciences](http://www.itp.cas.cn/), supervised by Prof. [Pan Zhang](http://home.itp.ac.cn/~panzhang/). My research interests lie at the interdisciplinary field among Statistical Physics, Quantum Computing and Tensor Network algorithms.

Here you can find my [CV](files/CV.pdf) and [Google Scholar Profile](https://scholar.google.com/citations?user=ZDEkIDsAAAAJ&hl).

<!--  **Notification**: the former ITP email address (panfeng@itp.ac.cn/panfeng@mail.itp.ac.cn) will soon be taken back, contact me through fengpan1994@gmail.com instead. -->

## Research Highlights

### Classical simulation of Sycamore quantum supremacy circuits.
After Google's random quantum circuit (RQC) sampling experiment in 2019, debates about how many time a classical device need to reproduce Goggle's computational task have never stopped. In this [PRL](https://doi.org/10.1103/PhysRevLett.128.030501) editors' suggestion paper, we use *big-head* method which is based on tensor network to classically generate over one million correlated bitstrings with exact amplitudes to spoof linear cross-entropy benchmark (XEB). The XEB fidelity of this sample is 73.9% which is much higher than Goggle's (0.2%). The running time of this simulation is around 5 days in a 60 NVIDIA V100 graphical processing units (GPUs). In this recent [PRL](https://doi.org/10.1103/PhysRevLett.129.090502) editors' suggestion paper, we use another tensor network based algorithm, *sparse-state contraction*, and low-rank detecting methods to classically reproduce exactly the same task as Goggle did in a computational cluster with 512 NVIDIA V100 GPUs in 15 hours. This simulation sampled over one million uncorrelated bitstrings with estimated fidelity 0.37%. We also estimate that if this simulation can be implemented in a high-end supercomputer with performance of exaFLOPS, the simulation time can be reduced to several seconds, which is smaller than the quantum simulation time. 

### Approximate/exact contraction method for arbitrary tensor networks.
Most applications of tensor networks into physical problems deal with lattice systems with organized connections. But what if the physical systems we care about are ones with arbitrary topologies? In this [PRL](https://link.aps.org/doi/10.1103/PhysRevLett.125.060503) paper, we investigate the solution by introducing Matrix Product State (MPS) calculus algorithm. This algorithm splits every tensor in TN into MPS, and contract them by a DMRG-like scheme, which keeps MPS form of the resulting tensor after each contraction. By adjusting the bond dimension of physical and virtual bonds, this algorithm can flexibly trade accuracy for contraction complexity. We use this algorithm into spin-glass models and quantum circuit simulations, which gives exciting results.  

### Machine learning assisted method for solving problems of statistical mechanics.
Machine learning algorithms have been made a powerful toolbox for physical research. In this [PRE](https://link.aps.org/doi/10.1103/PhysRevE.103.012103) paper, we use Varational Autoregressive models (VANs) combining the feedback vertex set (FVS) to deal with problems of statistical mechanics in spin-glass and combinatorial optimization. VANs are belong to generative models in ML and they hold a exact expression of the joint probability distribution over all variables, which is exactly physical problems need. The results are better than ones given by traditional variational and mean-field methods by a large margin.




<!-- This is the front page of a website that is powered by the [academicpages template](https://github.com/academicpages/academicpages.github.io) and hosted on GitHub pages. [GitHub pages](https://pages.github.com) is a free service in which websites are built and hosted from code and data stored in a GitHub repository, automatically updating when a new commit is made to the respository. This template was forked from the [Minimal Mistakes Jekyll Theme](https://mmistakes.github.io/minimal-mistakes/) created by Michael Rose, and then extended to support the kinds of content that academics have: publications, talks, teaching, a portfolio, blog posts, and a dynamically-generated CV. You can fork [this repository](https://github.com/academicpages/academicpages.github.io) right now, modify the configuration and markdown files, add your own PDFs and other content, and have your own site for free, with no ads! An older version of this template powers my own personal website at [stuartgeiger.com](http://stuartgeiger.com), which uses [this Github repository](https://github.com/staeiou/staeiou.github.io).

A data-driven personal website
======
Like many other Jekyll-based GitHub Pages templates, academicpages makes you separate the website's content from its form. The content & metadata of your website are in structured markdown files, while various other files constitute the theme, specifying how to transform that content & metadata into HTML pages. You keep these various markdown (.md), YAML (.yml), HTML, and CSS files in a public GitHub repository. Each time you commit and push an update to the repository, the [GitHub pages](https://pages.github.com/) service creates static HTML pages based on these files, which are hosted on GitHub's servers free of charge.

Many of the features of dynamic content management systems (like Wordpress) can be achieved in this fashion, using a fraction of the computational resources and with far less vulnerability to hacking and DDoSing. You can also modify the theme to your heart's content without touching the content of your site. If you get to a point where you've broken something in Jekyll/HTML/CSS beyond repair, your markdown files describing your talks, publications, etc. are safe. You can rollback the changes or even delete the repository and start over -- just be sure to save the markdown files! Finally, you can also write scripts that process the structured data on the site, such as [this one](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.ipynb) that analyzes metadata in pages about talks to display [a map of every location you've given a talk](https://academicpages.github.io/talkmap.html).

Getting started
======
1. Register a GitHub account if you don't have one and confirm your e-mail (required!)
1. Fork [this repository](https://github.com/academicpages/academicpages.github.io) by clicking the "fork" button in the top right. 
1. Go to the repository's settings (rightmost item in the tabs that start with "Code", should be below "Unwatch"). Rename the repository "[your GitHub username].github.io", which will also be your website's URL.
1. Set site-wide configuration and create content & metadata (see below -- also see [this set of diffs](http://archive.is/3TPas) showing what files were changed to set up [an example site](https://getorg-testacct.github.io) for a user with the username "getorg-testacct")
1. Upload any files (like PDFs, .zip files, etc.) to the files/ directory. They will appear at https://[your GitHub username].github.io/files/example.pdf.  
1. Check status by going to the repository settings, in the "GitHub pages" section

Site-wide configuration
------
The main configuration file for the site is in the base directory in [_config.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_config.yml), which defines the content in the sidebars and other site-wide features. You will need to replace the default variables with ones about yourself and your site's github repository. The configuration file for the top menu is in [_data/navigation.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_data/navigation.yml). For example, if you don't have a portfolio or blog posts, you can remove those items from that navigation.yml file to remove them from the header. 

Create content & metadata
------
For site content, there is one markdown file for each type of content, which are stored in directories like _publications, _talks, _posts, _teaching, or _pages. For example, each talk is a markdown file in the [_talks directory](https://github.com/academicpages/academicpages.github.io/tree/master/_talks). At the top of each markdown file is structured data in YAML about the talk, which the theme will parse to do lots of cool stuff. The same structured data about a talk is used to generate the list of talks on the [Talks page](https://academicpages.github.io/talks), each [individual page](https://academicpages.github.io/talks/2012-03-01-talk-1) for specific talks, the talks section for the [CV page](https://academicpages.github.io/cv), and the [map of places you've given a talk](https://academicpages.github.io/talkmap.html) (if you run this [python file](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.py) or [Jupyter notebook](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.ipynb), which creates the HTML for the map based on the contents of the _talks directory).

**Markdown generator**

I have also created [a set of Jupyter notebooks](https://github.com/academicpages/academicpages.github.io/tree/master/markdown_generator
) that converts a CSV containing structured data about talks or presentations into individual markdown files that will be properly formatted for the academicpages template. The sample CSVs in that directory are the ones I used to create my own personal website at stuartgeiger.com. My usual workflow is that I keep a spreadsheet of my publications and talks, then run the code in these notebooks to generate the markdown files, then commit and push them to the GitHub repository.

How to edit your site's GitHub repository
------
Many people use a git client to create files on their local computer and then push them to GitHub's servers. If you are not familiar with git, you can directly edit these configuration and markdown files directly in the github.com interface. Navigate to a file (like [this one](https://github.com/academicpages/academicpages.github.io/blob/master/_talks/2012-03-01-talk-1.md) and click the pencil icon in the top right of the content preview (to the right of the "Raw | Blame | History" buttons). You can delete a file by clicking the trashcan icon to the right of the pencil icon. You can also create new files or upload files by navigating to a directory and clicking the "Create new file" or "Upload files" buttons. 

Example: editing a markdown file for a talk
![Editing a markdown file for a talk](/images/editing-talk.png)

For more info
------
More info about configuring academicpages can be found in [the guide](https://academicpages.github.io/markdown/). The [guides for the Minimal Mistakes theme](https://mmistakes.github.io/minimal-mistakes/docs/configuration/) (which this theme was forked from) might also be helpful. -->
