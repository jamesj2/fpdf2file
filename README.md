# FPDF Image

Original written @ http://www.fpdf.org/en/script/script76.php

## Description

The standard FPDF class builds the document entirely in memory, which can be problematic for large documents. This extension saves the pages to the destination file as soon as they are finished, which solves the issue.

After you have created the object, call Open() with the name of the file:
```
$pdf = new FPDF2File();
$pdf->Open('doc.pdf');
```
and when the document is finished, call Output():
```
$pdf->Output();
```
Note: you can't use the AliasNbPages() method with this extension.
