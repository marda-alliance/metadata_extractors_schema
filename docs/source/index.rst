MaRDA Metadata Extractors Schema
================================

A repository at |MMESchemaRepo|_, containing the |LinkML|_-based schemas backing the |MMERegistryRepo|_.

The schemas implemented here are machine-actionable. They are used by the `Registry <https://marda-registry.fly.dev/>`_ to validate entries; a reference implementation demonstrating their pracical use is shown in the |MMEAPIRepo|_.

Contents
````````
The repository contains a schema two user-facing classes:

- The |FileType|_ class, used to specify the types of files passed to the extractors by users.
- The |Extractor|_ class, used to specify the download, installation, and usage instructions, allowing for machine execution of the defined extractor/parser code, as well as a list of :class:`FileTypes` compatible with the :class:`Extractor`.


.. toctree::
   :maxdepth: 1
   :caption: Usage Docs
   :hidden:

   Usage<usage>
   Contributing<contributing>

.. toctree::
   :maxdepth: 0
   :caption: Schema Docs
   :hidden:

   mme_schema/FileType
   mme_schema/Extractor

.. toctree::
   :maxdepth: 3
   :caption: Autogenerated Docs
   :hidden:
   :glob:

   mme_schema/index



.. |MMESchemaRepo| image:: https://badgen.net/static/marda-alliance/metadata_extractors_schema/?icon=github

.. _MMESchemaRepo: https://github.com/marda-alliance/metadata_extractors_schema/

.. |MMERegistryRepo| image:: https://badgen.net/static/marda-alliance/metadata_extractors_registry/?icon=github

.. _MMERegistryRepo: https://github.com/marda-alliance/metadata_extractors_registry/

.. |MMEAPIRepo| image:: https://badgen.net/static/marda-alliance/metadata_extractors_api/?icon=github

.. _MMEAPIRepo: https://github.com/marda-alliance/metadata_extractors_api/

.. |LinkML| replace:: :mod:`LinkML`

.. _LinkML: https://linkml.io/linkml/

.. |FileType| replace:: :class:`FileType`

.. _FileType: mme_schema/FileType.html#class-filetype

.. |Extractor| replace:: :class:`Extractor`

.. _Extractor: mme_schema/Extractor.html#class-extractor
