> Note: As of May 2024, this repository has been archived and the development of the metadata extractor schema continues under the [datatractor/schema](https://github.com/datatractor/schema) project.




<div align="center" style="padding-bottom: 1em;">
<img width="100px" align="center" src="https://avatars.githubusercontent.com/u/74017645?s=200&v=4">
</div>

# <div align="center">MaRDA Metadata Extractors: Schema</div>
<div align="center">

[![Documentation](https://badgen.net/badge/docs/marda-alliance.github.io/blue?icon=firefox)](https://marda-alliance.github.io/metadata_extractors_schema)
![Github status](https://badgen.net/github/checks/marda-alliance/metadata_extractors_schema/?icon=github)

</div>

A repository containing the [LinkML](https://linkml.io/linkml/)-based schemas backing the
MaRDA Metadata Extractors [Registry](https://github.com/marda-alliance/metadata_extractors_registry/)
and [API](https://github.com/marda-alliance/metadata_extractors_api/).

The schemas implemented here are machine-actionable. They are used by the [Registry](https://github.com/marda-alliance/metadata_extractors_registry/) to validate entries; a reference implementation demonstrating
their pracical use is shown in the [API](https://github.com/marda-alliance/metadata_extractors_api/).

## Contents
The repository contains two user-facing schemas:

- ``FileType`` schema, used to specify the types of files passed to the extractors by users.
  The schema definition is located in [``filetype.yaml``](./schemas/filetype.yaml).

- ``Extractor`` schema, used to specify the download, installation, and usage instructions,
  allowing for machine execution of the defined extractor/parser code, as well as a list of
  ``FileTypes`` compatible with the ``Extractor``.
  The schema definition is located in [``extractor.yaml``](./schemas/extractor.yaml).

## Usage
### Validation
The schema definitions contained in this repository can be used to locally validate your own
``FileTypes`` and ``Extractors``. Several examples are provided for this purpose in the
[``examples`` folder](./examples/).

To get started, first make sure LinkML is installed in your python environment. You may use
the provided ``requirements.txt`` file for this purpose:

```
pip install -r requirements.txt
```

Then, you can check the validity of your filetype or extractor definition against the provided
schemas using ``linkml-validate``. For example, to validate the provided example filetype definition
in [``FileType-netcdf.yaml``](./examples/FileType-netcdf.yaml) against the ``FileType`` class
from ``schemas/filetype.yaml``, run:

```
linkml-validate -s schemas/filetype.yaml -C FileType examples/FileType-netcdf.yaml
```

If successful, you should see "``✓ No problems found``" returned by ``linkml-validate``.

### Translation

The LinkML schemas provided here can be automatically translated to other formats, including
JSONSchema, Python dataclasses, or Pydantic classes:

```
gen-json-schema schemas/extractor.yaml >> extractor.json
gen-python schemas/filetype.yaml >> filetype.py
gen-pydantic schemas/extractor.yaml >> extractor.py
```

The generated files can be used in downstream codes such as in the [validation function](https://github.com/marda-alliance/metadata_extractors_registry/blob/main/tasks.py#L33)
of the [MaRDA Metadata Extractors Registry](https://github.com/marda-alliance/metadata_extractors_registry).

## Contributing

Contributions are welcome. We pledge to follow the [Contributor Covenant Code of Conduct](https://www.contributor-covenant.org/version/2/1/code_of_conduct/).

If you wish to contribute a new `FileType` or a new `Extractor` to the Registry, please open a pull request at [the Registry repo](https://github.com/marda-alliance/metadata_extractors_registry).

If you have any suggestions, technical queries, or a feature request related
to the schemas, please do not hesitate to open an issue in this repository. For general
questions related to the MaRDA Metadata Extractors WG, please use the [discussion board](https://github.com/marda-alliance/metadata_extractors/discussions).
