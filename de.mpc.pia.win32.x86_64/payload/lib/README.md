PIA - Protein Inference Algorithms
==================================

[![Build Status](https://travis-ci.org/mpc-bioinformatics/pia.svg?branch=master)](https://travis-ci.org/mpc-bioinformatics/pia)

PIA is a toolbox for MS based protein inference and identification analysis.

PIA allows you to inspect the results of common proteomics spectrum
identification search engines, combine them seamlessly and conduct statistical 
analyses.
The main focus of PIA lays on the integrated inference algorithms, i.e.
concluding the proteins from a set of identified spectra. But it also allows
you to inspect your peptide spectrum matches, calculate FDR values across
different search engine results and visualize the correspondence between PSMs,
peptides and proteins.

![PIA - Logo](https://github.com/mpc-bioinformatics/pia/wiki/pia_logo.png)


PIA in a nutshell
=================

Most search engines for protein identification in MS/MS experiments return
protein lists, although the actual search yields a set of peptide spectrum
matches (PSMs). The step from PSMs to proteins is called “protein inference”.
If a set of identified PSMs supports the detection of more than one protein in
the searched database (“protein ambiguity”), usually only one representative
accession is reported. These representatives may differ according to the used
search engine and settings. Thus the protein lists of different search engines
generally cannot be compared with one another. PSMs of complementary search
engines are often combined to enhance the number of reported proteins or to
verify the evidence of a peptide, which is improved by detection with distinct
algorithms.

We developed an algorithm suite written in Java, including a fully
parametrisable web-interface (using JavaServer Faces), which combines PSMs from
different experiments and/or search engines, and reports consistent and thus
comparable results. None of the parameters for the inference, like filtering or
scoring, are fixed as in prior approaches, but held as flexible as possible, to
allow for any adjustments needed by the user.

PIA can be called via the command line, in the workflow environment KNIME or
using a web-interface (which requires an installation of a web server, but feel
free to test it using the test server).


Download
========
For how to install and run PIA inside KNIME see [the wiki about PIA in KNIME](https://github.com/mpc-bioinformatics/pia/wiki/Running-PIA-via-KNIME).

Download the latest released version [here](https://github.com/mpc-bioinformatics/pia/releases/latest).


Documentation
=============

For documentation please refer to the Wiki (https://github.com/mpc-bioinformatics/pia/wiki) on github.


Problems, Bugs and Issues
=========================
If you have any problems with PIA or find bugs and other issues, please use the
issue tracker of github (https://github.com/mpc-bioinformatics/pia/issues).


Citation and Publication
========================
If you found PIA useful for your work, please cite the following publication:

http://www.ncbi.nlm.nih.gov/pubmed/25938255


Test Server
===

We provide a test installation of the web interface on http://134.147.84.213:8080/pia/

In your own interest, don't sent any sensitive research data to this server!
