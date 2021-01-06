Subtopic -  top officials’ salaries

The files 'retribuicions.xls' and 'retribuicions.ods' are the same, in two different formats (I was not sure which one was working better for Google Drive).
They correspond to the salaries in the "Departament d'Agricultura, Ramaderia, Pesca, Alimentació i Medi Natural" and "Departament de Cultura", on these two links:

http://www20.gencat.cat/docs/DAR/DE_Departament/DE30_Dades_obertes/Documents/Fitxers_estatics/retribucions_alts_carrecs_agricultura.pdf
http://www20.gencat.cat/docs/CulturaDepartament/SID/Transparencia/Estatics/Retribucions%20alts%20carrecs%20i%20eventuals%20Dept%20CU.pdf

I started doing this using the Google Drive Optical Character Recognition (OCR), in order to avoid typing all the values.

I found out that for the specific documents that I evaluated, the conversion to text works quite well, recognizing most of the characters. However, the structure of the vectorial file is quite 'messy', requiring some work to double check the structure and some 'copy paste'.

    Here were the steps I have taken to convert two documents from scanned pdfs with a non normalized structure, to a proper table in a spreadhseet.

    Import the pdf to google drive, but first set the importing options to "convert to text when uploading" (this is very important!)

    Open the document in Google drive and download it to a local file on the drive. After messing around a bit, I found out that the best option was to choose "RTF" (rich text format) as exporting format.

    Open the document on a text editor, and understand how it is organized (by comparing with the original image). On the first pdf I was lucky to have the data organized by columns, so I could copy it, column by column, to the spreadsheet. On the second document, I was not so lucky, because the data was organized in pairs of two rows (I have no idea why the OCR algorithm is behaving differently in the two cases)

    "tidy" up the table in excel, for instance by removing repeated headers, removing text from numerical cells, and sorting out the "." and "," convention for decimals (the last points are extremely important, if you want to do calculations). This is generally quite quick, because you can use "find and replace", multiple selection, etc.

    Sort out some misrecognized or missing characters, by comparing with the original image.

The final result should be a relational table with data organized by rows and columns, that can be used in a spreadsheet, exported to a database, and serve as basis for calculations and charts.