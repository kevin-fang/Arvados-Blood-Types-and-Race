# Formatting from BOOGIE directly from a compressed file

In this folder, the BOOGIEFormat.java program takes an zipped GFF file (in the GZIP format) and formats it.

To run BOOGIEFormat by itself (note that this does not run the code through BOOGIE and does not unzip the file, it merely converts the format from GFF to a style that BOOGIE can parse), compile BOOGIEFormat.java and call it "BoogieFormat.class" or something similar. Run the following command:

`java BOOGIEFormat <input name.gz> > <output name>`

Note that the `>` is needed because the results are printed to the standard output, so they need to be piped to another file.

Then, BOOGIE can be called directly on the output. 