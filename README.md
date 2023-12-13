# ediarum.AVHR.data-model

Version 1.0 from 22.11.2023

By Stefan Dumont, Tobias Kraft, Christian Thomas, Susanne Haaf, Jan Wierzoch

## Overview

This repository contains the definition of the data model of the edition humboldt digital (ehd): 

* ediarum.avhr.odd: General data model for edited texts of the ehd (based on ediarum.BASE)
* ediarum.avhr.register.odd: Data model for index entries (based on ediarum.REGISTER)
* ediarum.avhr.api.odd: Data model for the published versions of the edited texts (based on ediarum.avhr.odd)
* ediarum.abhr.api.articles.odd: Data model for the research articles

As noted above, most of the data models are based on generic data models, like [ediarum.BASE.data-model](https://github.com/ediarum/ediarum.BASE.data-model) and the [Base Format of the German Text Archive](https://deutschestextarchiv.de/doku/basisformat/) (DTABf). The data models are therefore formally derived from these models using ODD chaining, e.g. the (compiled) ediarum.BASE ODD is specified as the source schema in the ODD (in `schemaSpec/@source`). 

The ODD file that specifies the changes for the API output / public data publication is necessary, because internal IDs of persons, locations etc. are resolved into URIs in the API / data publication and, if available, supplemented with URIs from authority files.

The "dist" folder contains for each of the ODD files:
* the Relax NG file, which can be integrated as a schema in Oxygen XML Author and other XML-based software in order to validate XML files against it
* the compiled ODD file, which can be used as a starting point for creating ODD files for project-specific adaptations and additions of ediarum.BASE.

## Contact 

[Stefan Dumont, TELOTA/BBAW](https://www.bbaw.de/die-akademie/mitarbeiterinnen-mitarbeiter/dumont-stefan)

## Citation recommendation

Stefan Dumont, Tobias Kraft, Christian Thomas, Susanne Haaf, Jan Wierzoch: ediarum.AVHR.data-model. Data model of the edition humboldt digital. Berlin-Brandenburg Academy of Sciences and Humanities. Version 1.0 from 22.11.2023. 

## License 

This work is available under the [Creative Commons Attribution 4.0 International License (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/)