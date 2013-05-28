marbl-ead
=======

EAD finding aids tagged with named entity URIs for work in the Networking Belfast project.


-----

This fork of repository was created for EAD XML enhancement work being done 
as part of the `Digital Scholarship Commons`_ project `Networking the Belfast Group`_ on resources from 
`Manuscripts, Archives, and Rare Book Library`_ (MARBL).

.. _Digital Scholarship Commons: http://disc.library.emory.edu/
.. _Networking the Belfast Group: http://web.library.emory.edu/disc/projects/networking-belfast-group
.. _Manuscripts, Archives, and Rare Book Library: http://marbl.library.emory.edu

The master branch contains the original MARBL EAD files (as well as any updates made by MARBL during the project). 
The developer branch contains the tagged EAD files. 

Project contributors should create a branch for the XML file they are working on, tag names, and link to 
appropriate authority record URIs (VIAF, GeoNames.org, DBpedia), and commit to the appropriate branch. 

MARBL staff will review the diffs between the developer and master branches before pulling the tagged EAD into MARBL's live sites.

-----

Tags will be added using the Oxygen XML editor using the `Namedropper-oxygen`_ and/or from the command line
using the `Namedropper-python`_ tools. After changes are committed, those creating tags should provide
line-level comments on questionable tags using the GitHub interface.

.. _Namedropper-oxygen: https://github.com/emory-libraries-disc/namedropper-oxygen
.. _Namedropper-python: https://github.com/emory-libraries-disc/namedropper-py
