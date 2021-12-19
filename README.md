# Cadratin

## XML file structure

According the the official documentation:

> Documents in OpenDocument file format are stored as compressed zip archives that contain XML files. To view these XML files, you can open the OpenDocument file with an unzip program. The following files and directories are contained within the OpenDocument files:

1. The text content of the document is located in `content.xml`
2. The file `meta.xml` contains the meta information of the document [^1]

[^1]: Values mentioning printing (`meta:printed-by` and `meta:print-date`) are left empty
