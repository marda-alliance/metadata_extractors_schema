# MaRDA Extractors WG Schema Development

A place for the [Metadata Exctractors WG](https://github.com/marda-alliance/metadata_extractors/) to work on ideas regarding schema development.

## Initial work

Some initial schemas have been sketched out with [LinkML](https://linkml.io/linkml/), e.g., `filetype.yml` with the example data `biologic_mpr.yml`.
They can be used as follows, after installing LinkML (`pip install -r requirements.txt` in a fresh environment)

- Generate a JSONSchema version of the file type schema:
  ```
  gen-json-schema filetype.yml >> filetype.json
  ```

- Generate pydantic or dataclass models for the FileType schema:
  ```
  gen-python filetype.yml >> filetype.py
  ```

- Validate example data against the schema:
  ```
  linkml-validate -s filetype.yml -C FileType biologic_mpr.yml
  ```
