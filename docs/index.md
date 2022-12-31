
# filetype


**metamodel version:** 1.7.0

**version:** None





### Classes

 * [FileType](FileType.md) - A specific encoding of data for storage purposes, defined by a set of common characteristics and expectations, that can be assumed for all files of a given file type.

### Mixins


### Slots

 * [➞associated_instruments](fileType__associated_instruments.md) - Any instrument, or class of instruments, that typically create the data encoded into such files.
 * [➞associated_software](fileType__associated_software.md) - Any software (proprietary or otherwise) that produces such files.
 * [➞associated_standards](fileType__associated_standards.md) - If this is a subformat that follows a particular well-defined standard, e.g., CIF, NeXus, then it can be listed here.
 * [➞associated_vendors](fileType__associated_vendors.md) - If this file type is associated with particular software or instrument vendors, they can be listed here.
 * [➞base_formats](fileType__base_formats.md) - If this format uses any particular underlying generic formats, e.g., CSV, JSON, HDF5, then they can be listed here.
 * [➞description](fileType__description.md) - A human-readable outline of the file type, its format, data content and uses.
 * [➞id](fileType__id.md) - A unique identifier for the format within the MaRDA registry namespace, this should be a shorthand label rather than a UUID. Only lower-case alphanumeric and dash ("-") characters are permitted.
 * [➞name](fileType__name.md) - A recognisable name for the format.
 * [➞subject](fileType__subject.md) - Any keywords, phrases or classification codes that are relevant to the file type, e.g., particular scientific domains of applicability, or experimental techniques.

### Enums


### Subsets


### Types


#### Built in

 * **Bool**
 * **Decimal**
 * **ElementIdentifier**
 * **NCName**
 * **NodeIdentifier**
 * **URI**
 * **URIorCURIE**
 * **XSDDate**
 * **XSDDateTime**
 * **XSDTime**
 * **float**
 * **int**
 * **str**

#### Defined

 * [Boolean](types/Boolean.md)  (**Bool**)  - A binary (true or false) value
 * [Date](types/Date.md)  (**XSDDate**)  - a date (year, month and day) in an idealized calendar
 * [DateOrDatetime](types/DateOrDatetime.md)  (**str**)  - Either a date or a datetime
 * [Datetime](types/Datetime.md)  (**XSDDateTime**)  - The combination of a date and time
 * [Decimal](types/Decimal.md)  (**Decimal**)  - A real number with arbitrary precision that conforms to the xsd:decimal specification
 * [Double](types/Double.md)  (**float**)  - A real number that conforms to the xsd:double specification
 * [Float](types/Float.md)  (**float**)  - A real number that conforms to the xsd:float specification
 * [Integer](types/Integer.md)  (**int**)  - An integer
 * [Ncname](types/Ncname.md)  (**NCName**)  - Prefix part of CURIE
 * [Nodeidentifier](types/Nodeidentifier.md)  (**NodeIdentifier**)  - A URI, CURIE or BNODE that represents a node in a model.
 * [Objectidentifier](types/Objectidentifier.md)  (**ElementIdentifier**)  - A URI or CURIE that represents an object in the model.
 * [String](types/String.md)  (**str**)  - A character string
 * [Time](types/Time.md)  (**XSDTime**)  - A time object represents a (local) time of day, independent of any particular day
 * [Uri](types/Uri.md)  (**URI**)  - a complete URI
 * [Uriorcurie](types/Uriorcurie.md)  (**URIorCURIE**)  - a URI or a CURIE
