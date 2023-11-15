# ediarum.AVHR.data-model

**WIP: Currently still work in progress**

This repository contains the definition of the data model of the edition humboldt digital (ediarum.AVHR.odd). The data model is based on ediarum.BASE. It is therefore also formally derived from this (using ODD chaining), i.e. the (compiled) ediarum.BASE ODD is specified as the source schema in the ODD. 

There is also a second ODD file that specifies the changes for the API output / public data publication compared to the internally used schema. For example, internal IDs of persons, locations etc. are resolved into URIs in the API / data publication and, if available, supplemented with URIs from authority files.

The "dist" folder contains for each of the two ODD files:
* the Relax NG file, which can be integrated as a schema in Oxygen XML Author and other XML-based software in order to validate XML files against it
* the compiled ODD file, which can be used as a starting point for creating ODD files for project-specific adaptations and additions of ediarum.BASE.
