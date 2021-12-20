# Cadratin

## XML file structure

According the the official documentation:

> Documents in OpenDocument file format are stored as compressed zip archives that contain XML files. To view these XML files, you can open the OpenDocument file with an unzip program. The following files and directories are contained within the OpenDocument files:

1. The text content of the document is located in `content.xml`
2. The file `meta.xml` contains the meta information of the document [^1]
3. The file `settings.xml` contains further information about the settings for this document [^2]
4. the styles applied to the document can be find in the file `styles.xml`
5. The `META-INF/manifest.xml` file describes the structure of the XML file

Additional files are contained in the packed file format:

1. The `manifest.rdf` file lists files which are contained in the document that contain RDF metadata, such as `content.xml` and `styles.xml`
2. The `mimetype` file is containing the ASCII encoded MIME media type associated with the document

[^1]: Values mentioning printing (`meta:printed-by` and `meta:print-date`) are left empty
[^2]: Some values about printing (`config:name="PrinterName"` and `config:name="PrinterSetup"`) are left empty
