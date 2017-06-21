Files in directory:
exporter.py - Script to retrieve JSON and store in MS word doc
test_exports.py - Test for exporter.py using pytest
requirements.txt - Dependencies to install for the script
results_reference.docx - Reference of transcript to compare the script against


To install dependencies:
Refer requirements.txt

To run the script:
"python exporter.py <transaction ID> <API Key>"
Results are dumped in results_created.docx

To run test:
"pytest"
The test will create an MS doc file of the transcript in results_created.docx.
It will then compare the time stamp and transcript of each paragraph in the newly created document with the reference results document.
Please note that it does not test the word confidence.


Note: It looks like some of the red highlighting in the reference document provided is incorrect.
For example, in the last transcript, 'am' is highlighted in red but has a confidence of 0.776.

