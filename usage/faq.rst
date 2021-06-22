##############################
FAQ
##############################

====================================================
Data Import
====================================================
------------------------------------------------
How do I import data in VCF format?
------------------------------------------------
**A:**
VCFs must first be converted to MAF format.
If you're comfortable programming, use vcf2maf_.
If you are not, please `contact me via email`_.

We are currently working on building better workflows for importing VCFs to CRUX for non-programmers.

====================================================
Analysis
====================================================
------------------------------------------------
What are 'dubious genes'?
------------------------------------------------
**A:**
A list of genes which are frequently mutated in somatic cancer datasets but that are unlikely to drive disease.
These genes can be excluded from analysis in CRUX.
The genelist is described in the somaticflags_ package.

====================================================
Tool development
====================================================
------------------------------------------------
I have an idea for a new feature?
------------------------------------------------
Submit your feature request here_
or `contact me via email`_

------------------------------------------------
Where do I report bugs and other odd behaviour?
------------------------------------------------
Submit your issue here_
or `contact me via email`_ at

====================================================
Miscellaneous
====================================================
------------------------------------------------
My question isn't here. What do I do?
------------------------------------------------
**A:**
Please `contact me via email`_.


.. _somaticflags: https://github.com/CCICB/somaticflags/blob/main/README.md/
.. _vcf2maf: https://github.com/mskcc/vcf2maf/
.. _here: https://github.com/CCICB/CRUX/issues/
.. _`contact me via email`: selkamand@ccia.org.au
