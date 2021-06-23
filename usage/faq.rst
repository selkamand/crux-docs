##############################
FAQ
##############################

====================================================
Data Import
====================================================
------------------------------------------------
How do I import data in VCF format?
------------------------------------------------
VCFs must first be converted to MAF format.
If you're comfortable programming, use vcf2maf_.
If you are not, please `contact us`_.

We are currently working on building better workflows for importing VCFs to CRUX for non-programmers.

====================================================
Analysis
====================================================
------------------------------------------------
What are 'dubious genes'?
------------------------------------------------
A list of genes which are frequently mutated in somatic cancer datasets but that are unlikely to drive disease.
These genes can be excluded from analysis in CRUX.
The genelist is described in the somaticflags_ package.

------------------------------------------------
Why is the text in my figures so small?
------------------------------------------------
Most visualisation modules have options to set text-size.
Sometimes increasing the font-size will cause parts of the text to be cut off.
When this happens, you have two options.
Look for an option to increase **margins** (e.g **Margin: genes** if working with an oncoplot).
Alternatively, keep the font-size small, download the plot in a *vector-based format* such as a PDF (Illustrator) or SVG (Inkscape) and edit the text size in an 3rd party program.


Hopefully, we will one day have the options to set 'Margins' for all plots.

====================================================
Tool development
====================================================
--------------------------------------------------------------------------------
I have an idea for a new feature. Who should I tell?
--------------------------------------------------------------------------------
Submit your feature request here_
or `contact us`_

--------------------------------------------------------------------------------
Where do I report bugs and other odd behaviour?
--------------------------------------------------------------------------------
Submit your issue here_
or `contact us`_

====================================================
Miscellaneous
====================================================
------------------------------------------------
My question isn't here. What do I do?
------------------------------------------------
Submit your issue here_ or
`contact us`_.


.. _somaticflags: https://github.com/CCICB/somaticflags/blob/main/README.md/
.. _vcf2maf: https://github.com/mskcc/vcf2maf/
.. _here: https://github.com/CCICB/CRUX/issues/
.. _`contact us`: selkamand@ccia.org.au
