marbl-ead
=========

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

**Instructions**

Tags will be added using the Oxygen XML editor using the `Namedropper-oxygen`_ and/or from the command line
using the `Namedropper-python`_ tools. After changes are committed, those creating tags should provide
line-level comments on questionable tags using the GitHub interface.

.. _Namedropper-oxygen: https://github.com/emory-libraries-disc/namedropper-oxygen
.. _Namedropper-python: https://github.com/emory-libraries-disc/namedropper-py

Sections of EAD documents to tag should be prioritized based on what the findingaids
software currently supports exposing via RDFa:

* It is important to tag origination name if it contains a personal or family
  name (``archdesc/did/origination``).
* Semantic data generation is currently supported for ``bioghist``, ``indexentry``,
  correspondence series, and series with belfast group sheet listings;
  other series/subseries can probably be skipped for now.
* In the ``bioghist`` (biographical/historical note), only tag names and places
  that are related to the origination or "main entry" person or organization;
  do not tag repeated instances of the main person or group associated with the
  collection.
* It is beneficial to tag names in the ``controlaccess`` / Selected Search
  Terms.
* If a series is about a person or group, tag the name in the ``unittitle``
  when possible (e.g., series 11 with Edna Longley materials in the
  Michael Longley collection).
