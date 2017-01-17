# PBS Caption Clean
This is a simple Python script that cleaning up caption files for PBS COVE ingestion. It removes characters that are known to cause ingestion failures.

When a caption file ingestion fails, usually the first thing I do is check the caption file for special characters.

This script only works with plain text caption files. If you're working with caption files that are not stored in plain text, you may want to check out [pycaption](https://github.com/pbs/pycaption) for converting caption files to PBS' preferred caption format (DFXP).

# Usage

    ./caption-clean [input-file] [output-file]

Below are some examples on how to use this script assuming you're running python from the command line.

If no output file is provided, it is copied to `myCaptionFile.xml.orig`

    ./caption-clean myCaptionFile.xml

## Find a charachter that isn't being remove?
If you're noticing a charachter that is probably the cause of a failed ingest, feel free to submit a pull request or open an issue on GitHub.
