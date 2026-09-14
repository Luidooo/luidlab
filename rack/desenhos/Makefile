# MR2020 drawing set:  make [pdf | imagens | preview | limpa]
# One master file (mr2020.tex) builds every sheet into mr2020.pdf.
# Compiles twice: sheets are placed on the page with remember picture.
MASTER := mr2020
SHEETS := $(wildcard [0-9][0-9]-*.tex)

pdf: $(MASTER).pdf
tudo: pdf

$(MASTER).pdf: $(MASTER).tex $(SHEETS) iso.sty params.tex
	@pdflatex -interaction=nonstopmode -halt-on-error $(MASTER).tex >/dev/null && \
	 pdflatex -interaction=nonstopmode -halt-on-error $(MASTER).tex >/dev/null || \
	  { pdflatex -interaction=nonstopmode $(MASTER).tex; exit 1; }
	@echo "  ->  $@"

# README images: sheet 01 (isometric view) and sheet 05 (rack unit layout)
imagens: $(MASTER).pdf
	@mkdir -p ../img
	@pdftoppm -png -r 150 -singlefile -f 1 -l 1 $(MASTER).pdf ../img/isometric-view
	@pdftoppm -png -r 150 -singlefile -f 5 -l 5 $(MASTER).pdf ../img/rack-unit-layout
	@echo "  ->  ../img/isometric-view.png  ../img/rack-unit-layout.png"

preview: $(MASTER).pdf
	@pdftoppm -png -r 140 $(MASTER).pdf preview

limpa:
	rm -f *.aux *.log *.out *.png

.PHONY: pdf tudo imagens preview limpa
