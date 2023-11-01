MaRDA Metadata Extractors Schema
================================

A repository at |MMESchemaRepo|_, containing the |LinkML|_-based schemas backing the MaRDA Metadata Extractors Registry and API.

The schemas implemented here are machine-actionable. They are used by the `Registry <https://github.com/marda-alliance/metadata_extractors_registry/>`_ to validate entries; a reference implementation demonstrating their pracical use is shown in the `API <https://github.com/marda-alliance/metadata_extractors_api/>`_.

Contents
````````
The repository contains two user-facing schemas:

- The |FileType|_ schema, used to specify the types of files passed to the extractors by users.
- The |Extractor|_ schema, used to specify the download, installation, and usage instructions, allowing for machine execution of the defined extractor/parser code, as well as a list of :class:`FileTypes` compatible with the :class:`Extractor`.


.. toctree::
   :maxdepth: 1
   :caption: Usage Docs
   :hidden:

   Usage<usage>
   Contributing<contributing>

.. toctree::
   :maxdepth: 1
   :caption: Schema Docs
   :hidden:

   gen-doc/FileType
   gen-doc/Extractor

.. |MMESchemaRepo| image:: https://badgen.net/static/marda-alliance/metadata_extractors_schema/?icon=github

.. _MMESchemaRepo: https://github.com/marda-alliance/metadata_extractors_schema/

.. |LinkML| replace:: :mod:`LinkML`

.. _LinkML: https://linkml.io/linkml/

.. |FileType| replace:: :class:`FileType`

.. _FileType: filetype/filetype.html#class-filetype

.. |Extractor| replace:: :class:`Extractor`

.. _Extractor: extractor/extractor.html#class-extractor
