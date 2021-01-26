
# code
```
import os
os.chdir("/home/oujbih/Biblio/python/PDF_mo")    


from wand.image import Image
from PyPDF2 import PdfFileWriter, PdfFileReader

# my_pdf = Image(filename="main.pdf", resolution=150)
inputpdf = PdfFileReader(open("main.pdf", "rb"))
output = PdfFileWriter()
output.addPage(inputpdf.getPage(11))

with open("small.pdf", "wb") as outputStream:
    output.write(outputStream)
    
https://stackoverflow.com/questions/490195/split-a-multi-page-pdf-file-into-multiple-pdf-files-with-python
```
