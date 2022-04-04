## Shrinkpdf

PDF Size Reduce(compress) using Ghostscript at terminal. 
Here required 2 things for the process.

1. shrinkpdf.sh file
2. Installed `Ghostscript` in your machine

### Setup

1. Download the shrinkpdf.sh file from ![Here](http://www.alfredklomp.com/programming/shrinkpdf/shrinkpdf.sh)

2. Install `Ghostscript` in your machine if not installed

***For Mac : ***
`sudo brew install ghostscript`

***For Linux : ***

RedHat and derivatives :
`sudo yum install ghostscript`
Or on Debian:
`sudo apt-get install ghostscript`


### Process


To reduce your pdf file you need to pass 3 parameters

./shrinkpdf.sh [inputfile] [outputfile] [resolution_in_dpi]

1. [inputfile] : Actual Filename of the PDF that is to be converted
2. [outputfile] : New filename of the converted PDF
2. [resolution_in_dpi] : The DPI (resolution) for the output PDF. 
Output resolution defaults is : 72 . You can use your own choice like 150 dpi , 150 dpi etc.

N.B: Lower DPI is better but the quality will be worse

### Execute and Reduce PDF

***Step 1 :  ***

Make the `shrinkpdf.sh` file executable and give it permissions to execute by  bellow command

  ``sudo chmod +x shrinkpdf.sh``

Now your `shrinkpdf.sh` file is executable.

***Step 2 :  ***

So now you can execute the the `shrinkpdf.sh`

`sudo ./shrinkpdf.sh sample-pdf.pdf output.pdf 150`


More Detials :

http://www.alfredklomp.com/programming/shrinkpdf/
