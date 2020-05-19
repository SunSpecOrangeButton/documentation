# Orange Button Design

The following documentation is intended for application developers and technical users of the Sunspec Github Repos.
More information on data standard submittals is available at [orangebutton.io](http://orangebutton.io).

![OrangeButtonDesign](docs/OrangeButtonDesign.png)

## Solar Taxonomy ##

Two editions of the Taxonomy are available and described below.

**XBRL Taxonomy**

The Orange Button Taxonomy is defined using the XBRL standard. XBRL is the international standard for the electronic representation
of business reports.​ XBRL allows the definition, preparation and exchange of reporting information across organizational
boundaries. It does so in a manner that can be validated at every point in the process which is made possible through a 
number of interrelated technical ​specifications collectively referred to as the XBRL International Specification. These
specifications set out how to create and test the "metadata" parts of XBRL: taxonomies, concepts, and dimensions (tables),
as well as the "data" components: instances and facts.​ The XBRL specification allows data conforming to the taxonomy to be
defined in multiple formats including XML, JSON, and CSV. The Taxonomy itself if defined using an XML based specification.

**Open API Taxonomy**

The OpenAPI Specification (OAS) defines a standard, language-agnostic interface to RESTful APIs which allows both humans 
and computers to discover and understand the capabilities of the service without access to source code, documentation, or 
through network traffic inspection.

Please note that this is not necessarily synchronized with the XBRL Taxonomy at this point in time.

## Open Source Software ##

**Open API Editor**

The OB OpenAPI Editor is a web application that allows users to edit or create Orange Button compliant schemas in the
OpenAPI format. Schemas are created using standardized solar industry terms that are defined in the Solar Taxonomy. 
The editor allows the definitions in the Solar Taxonomy context to be used in the more easy-to-use JSON format, allowing 
for easier use in web service applications.

**Pyoblib**

pyoblib - includes an in memory data model, in memory meta-data about the solar taxonomy, and common tools (XML/JSON
input output, conversion, vaidation, identifier generation, etc...).  Pyoblib intentionally does not include an on disk
database (due to the large discrepancy on implementation intentions) although it may at a later date.  The core libraries
should leverage the Python standard library to the extent possible to minimize required dependencies.  The Solar Taxonomy
itself (an XSD based specification) is also published in the core shared area.  Python Programs may also be included
outside of the core libaries and the programs may be compatible with any python implementation.

**Orange Button Taxonomy Viewer (OBTV)**

The Orange Button Taxonomy Viewer allows for searching and displaying Orange Button Entrypoints, Concepts, Types, and
Units by non-XBRL.  OBTV is a Vue.js application and relies on Pyoblib to generate the underlying meta data required
at build time.

**Product Code Registry**

The Orange Button Product Code Registry is a web application containing registered product code strings allowing them
to be standardized throughout the industry. The registry holds name and identifier information regarding entities and
their products. It serves as a record keeper for the Orange Button compliant identifiers. The registry standardizes the
naming schema for consistency and easy accessibility.

**The status of the various components follows:**

- Solar XBRL Taxonomy: Available (v 2020-04-01)
- Solar Open API Taxonomy: Available but not versioned
- pyoblib: Available (v 1.0.3)
- OB Open API Editor: Available but not versioned
- Product Code Registry (front-end and server): Available
- Archive:
    - ob-python-xbrl-generator: Archived
    - open-api (legacy): Archived
- Other (not diagramed):
    - Clabot (Available)
    - Documentation
  
## XBRL Tools

An alternative method for processing Orange Button data is to use XBRL Tools. Please reach out to XBRL.US for more
information on obtaining the tools and/or their source code.
 
- Arelle: For XBRL experts the Arelle desktop software is a better option than OBTV - instructions are below.
Please note that for non-XBRL users OBTV is easier to use.

- Xule is a plugin to Arelle.  It allows for establishment of custome Data Quality rules that can be applied to XBRL
data.  

- The SEC database is an example of a working XBRL database that can be operated via Arelle.

- A PDF based guide is also available at [guide](https://sunspec.org/wp-content/uploads/2017/10/OrangeButtonTaxonomyGuideMay2018.pdf).
Please note that this has not been updated since the May 2018 Orange Button Taxonomy release so many of its details are 
incorrect.  However at a conceptual level the guide is still quite helpful.

## Getting started

Before working on Orange Button source code either the Individual or Corporate Contributors agreement must be signed.
Information is available at [Orange Button](https://orangebutton.io/community/).

For new repositories contact send an email to support@sunspec.org to vett the initial idea and create the repository.
Use the template-application repository as a starting point.  At a minimum the Apache 2.0 LICENSE file must be present.

For current repositories contact the repository facilitator to determine colloboration procedure.  Some repositories use
pull requests, as docuemnted in the community web page referenced above.  This may be covered in CONTRIBUTING.md.  Usually the name of the facilitator is obvious based on who is performing the commits but if not contact support@sunspec.org in order to find out the contact inforamtion.

## Archived programs

Historical Orange Button components include:
    - The Yeti Review tool is still available online however the Taxonomy loaded on Yeti is not updated. Use OBTV or Arelle instead.
    - ob-python-xbrl-generator was built before pyoblib and some of its concepts still work in pyoblib.  ob-python-xbrl-generateor no longer runs.
    - open-api ia historical prototype.  It has been replaced by the Open API Editor and should not be used.

## Useful Links

Orange Button Resources: [link](https://sunspec.org/orange-button-resources/)

SunSpec Alliance: [link](https://sunspec.org/)

XBRL: [link](https://www.xbrl.org/)

Orange Button Taxonomy Viewer (OBTV): [link](https://blubanyan.com/orange-button-taxonomy-viewer)

Arelle: [link](http://arelle.org/)

Xule: [link](https://github.com/DataQualityCommittee/dqc_us_rules/)

Solar Taxonomy PDF Based Guide: [link](https://sunspec.org/wp-content/uploads/2017/10/OrangeButtonTaxonomyGuideMay2018.pdf).  Please
note that this is not currently up to date but still can be used for conceptual purposes.
