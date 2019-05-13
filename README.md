# Orange Button Design

![OrangeButtonDesign](docs/OrangeButtonDesign.png)

**Three types of code are available:**

1. Orange Button Core Open Source is maintained by the Orange Button Open Source community.  It includes Apache 2.0 licensed libraries.  The projets are written in Python 3.x.  The main code library - pyoblib - includes an in memory data model, in memory meta-data about the solar taxonomy, and common tools (XML/JSON input output, conversion, vaidation, identifier generation, etc...).  Pyoblib intentionally does not include an on disk database (due to the large discrepancy on implementation intentions) although it may at a later date.  The core libraries should leverage the Python standard library to the extent possible to minimize required dependencies.  The Solar Taxonomy itself (an XSD based specification) is also published in the core shared area.  Python Programs may also be included outside of the core libaries and the programs may be compatible with any python implementation.
2. XBRL Open Source code may be leveraged on an as needed basis.  XBRL code is maintained outside of the Orange Button GitHub environment and is a partner open source community.  More information on XBRL is available at [XBRL](https://www.xbrl.org/) and [Arelle](http://arelle.org/).
3. A hypothetical design for an end to end program exists leveraging the open source libraries.  At this point in time no end to end edition exists although at least one of the sample programs could be leveraged.

**Currently only a portion of the source code is available.  The status of the various components follows:**

- pyoblib: Available (v 1.0.0)
- Solar Taxonomy: Available (v 1.3)
- Documentation: Available
- Sample Code / Orange Button Data: Available (more is needed)
- Product Code Registry: Available
- Archive: Available
    - ob-python-xbrl-generator: Archived
- Open API (Conceptual edition is built, format is not ratified)
- Arelle: Available
- Arelle Plugins: Available
- Xule: Available
- SEC Database upon request (not on GitHub)
- Other (not diagramed):
    - Clabot (Available)
    
##Solar Taxonomy, Arelle, and Yeti:

The official data specification for Orange Button is encompassed in the various XSD files in the solar-taxonomy GITHub repository.  However this is not easy to read or digest.  Thus it is better to use one of these tools:

- Arelle (v.1.3) - instructions below
- Yeti Review tool (v1.2) available at [yeti](https://yeti1.corefiling.com/) 
- A PDF based guide is also available at [guide](https://sunspec.org/wp-content/uploads/2017/10/OrangeButtonTaxonomyGuideMay2018.pdf).

**Arelle Instructions**

The desktop edition of Arelle can be downloaded (see useful links section below).  Alternatively contact [Jessie Deot](mailto:jessie@sunspec.org) to receive access to a hosted edition of Arelle.

## Getting started

Before working on Orange Button source code either the Individual or Corporate Contributors agreement must be signed.  Information is available at [Orange Button](https://sunspec.org/ob-open-source-community/).

For new repositories contact send an email to support@sunspec.org to vett the initial idea and create the repository.  Use the template-application repository as a starting point.  At a minimum the Apache 2.0 LICENSE file must be present.

For current repositories contact the repository facilitator to determine colloboration procedure.  Some repositories use pull requests, as docuemnted in the community web page referenced above.  This may be covered in CONTRIBUTING.md.  Usually the name of the facilitator is obvious based on who is performing the commits but if not contact support@sunspec.org in order to find out the contact inforamtion.

## Useful Links

Orange Button Resources: [link](https://sunspec.org/orange-button-resources/)

SunSpec Alliance: [link](https://sunspec.org/)

XBRL: [link](https://www.xbrl.org/)

Arelle: [link](http://arelle.org/)

Xule: [link](https://github.com/DataQualityCommittee/dqc_us_rules/)

Yeti Solar Taxonomy Review Tool: [link](https://yeti1.corefiling.com/)

Solar Taxonomy PDF Based Guide: [link](https://sunspec.org/wp-content/uploads/2017/10/OrangeButtonTaxonomyGuideMay2018.pdf)
