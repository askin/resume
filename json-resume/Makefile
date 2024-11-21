# all: index.html index.pdf index.docx index.txt
all: Askin_Ozgur_CV-en.pdf
pbx: Askin_Ozgur_CV-en-pbx.pdf
normal: Askin_Ozgur_CV-en-normal.pdf
html: public/index.html
# theme: ./node_modules/jsonresume-theme-autumn/
# theme = macchiato
theme = ../jsonresume-theme-autumn

Askin_Ozgur_CV-en.pdf: resume-all.json
	resume export Askin_Ozgur_CV-en.pdf --theme $(theme) -f pdf

Askin_Ozgur_CV-en-pbx.pdf: resume-pbx.json
	resume export Askin_Ozgur_CV-en-pbx.pdf --theme $(theme) -f pdf

Askin_Ozgur_CV-en-normal.pdf: resume.json
	resume export Askin_Ozgur_CV-en-n.pdf --theme $(theme) -f pdf

public/index.html: resume.json
	resume export public/index.html --theme $(theme) -f html

clean:
	rm -f *.html *.pdf *.docx *.txt
