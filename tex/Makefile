TARGET?=luecke_cv

PDFTEXOPTS = -halt-on-error -pdf -pvc

default: build

clean:
	rm -f *.acn *.acr *.alg *.aux *.bbl *.blg *.dvi *.glg *.glo *.gls *.ist *.lof *.log *.lol *.lot *.out *.pdf *.toc *.pdfsync *.gz *.tdo
build: 

	pdflatex $(TARGET).tex
#	latexmk $(PDFTEXOPTS) $(TARGET).tex
#	bibtex $(TARGET).aux
#	pdflatex $(PDFTEXOPTS) $(TARGET).tex
#	pdflatex $(PDFTEXOPTS) $(TARGET).tex

de:
	pdflatex $(TARGET)_de.tex

open: clean build
	xdg-open $(TARGET).pdf &
