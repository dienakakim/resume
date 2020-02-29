# Dien Tran's resume

My most up-to-date resume, built with HTML5, Vue, and Tailwind CSS.

## How to build

Install `nodejs` and then install `chromehtml2pdf` globally:

    npm i chromehtml2pdf -g

Then run the following command in the project directory to produce the PDF version:

    node -e "const{exec}=require('child_process');const path=require('path');const compilePDF=exec(`chromehtml2pdf -c --out output.pdf \"${path.resolve('newresume.html')}\"`);compilePDF.stdout.on('data', (data)=>console.log(data));compilePDF.stderr.on('data', (data)=>console.log(data));"

The filename should be `output.pdf` if done correctly.
