
# Class: FileType


A specific encoding of data for storage purposes, defined by a set of common characteristics and expectations, that can be assumed for all files of a given file type.

URI: [https://www.marda-alliance.org/extractors/filetype/FileType](https://www.marda-alliance.org/extractors/filetype/FileType)


[![img](https://yuml.me/diagram/nofunky;dir:TB/class/[FileType]<base_formats%200..*-%20[FileType&#124;id:string;name:string;description:string;associated_vendors:string%20*;associated_instruments:string%20*;associated_software:string%20*;associated_standards:string%20*;subject:string%20*])](https://yuml.me/diagram/nofunky;dir:TB/class/[FileType]<base_formats%200..*-%20[FileType&#124;id:string;name:string;description:string;associated_vendors:string%20*;associated_instruments:string%20*;associated_software:string%20*;associated_standards:string%20*;subject:string%20*])

## Referenced by Class

 *  **None** *[➞base_formats](fileType__base_formats.md)*  <sub>0..\*</sub>  **[FileType](FileType.md)**

## Attributes


### Own

 * [➞id](fileType__id.md)  <sub>1..1</sub>
     * Description: A unique identifier for the format within the MaRDA registry namespace, this should be a shorthand label rather than a UUID. Only lower-case alphanumeric and dash ("-") characters are permitted.
     * Range: [String](types/String.md)
 * [➞name](fileType__name.md)  <sub>1..1</sub>
     * Description: A recognisable name for the format.
     * Range: [String](types/String.md)
 * [➞description](fileType__description.md)  <sub>1..1</sub>
     * Description: A human-readable outline of the file type, its format, data content and uses.
     * Range: [String](types/String.md)
 * [➞associated_vendors](fileType__associated_vendors.md)  <sub>0..\*</sub>
     * Description: If this file type is associated with particular software or instrument vendors, they can be listed here.
     * Range: [String](types/String.md)
 * [➞associated_instruments](fileType__associated_instruments.md)  <sub>0..\*</sub>
     * Description: Any instrument, or class of instruments, that typically create the data encoded into such files.
     * Range: [String](types/String.md)
 * [➞associated_software](fileType__associated_software.md)  <sub>0..\*</sub>
     * Description: Any software (proprietary or otherwise) that produces such files.
     * Range: [String](types/String.md)
 * [➞base_formats](fileType__base_formats.md)  <sub>0..\*</sub>
     * Description: If this format uses any particular underlying generic formats, e.g., CSV, JSON, HDF5, then they can be listed here.
     * Range: [FileType](FileType.md)
 * [➞associated_standards](fileType__associated_standards.md)  <sub>0..\*</sub>
     * Description: If this is a subformat that follows a particular well-defined standard, e.g., CIF, NeXus, then it can be listed here.
     * Range: [String](types/String.md)
 * [➞subject](fileType__subject.md)  <sub>0..\*</sub>
     * Description: Any keywords, phrases or classification codes that are relevant to the file type, e.g., particular scientific domains of applicability, or experimental techniques.
     * Range: [String](types/String.md)

## Other properties

|  |  |  |
| --- | --- | --- |
| **Close Mappings:** | | schema_org:fileFormat |
|  | | schema_org:encodingFormat |
|  | | dublin_core:format |

