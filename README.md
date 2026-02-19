# Prezi2PDF
 Simple script to convert Prezi presentation into a PDF file. Can also download Prezi Videos

## Install dependencies
On Mac `python3 -m pip install -r requirements.txt` 

## How to use

1.  Run the script and enter the prezi url. `python3 prezi2pdf.py -u "YOUR_PREZI_URL"`  
2. The script will start downloading en converting it into a pdf file.

Note that the `YOUR_PREZI_URL` is a little ambigous. You should find the link that contains an ID of the following form: 12 symbols long, each either a digit, a lowercase letter, or a hyphen. 
Example: 
```
https://prezi.com/p/edit/vk713bm8qr-k/
```
In the case above, to get this link I have to open the presentation in the "Edit" mode.
If you only have the public viewing link (`https://prezi.com/p/<ID>/…`), the script picks up the 12-character ID automatically and you can still download the slides.
By default the download gets converted to PDF, but you can pass `-t pptx` if you prefer a PowerPoint output; the same `presentations/` folder will accumulate the `.pptx` file.