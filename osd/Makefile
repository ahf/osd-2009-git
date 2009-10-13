all: slides.pdf

clean:
	rm -f *.snm *.toc *.aux *.log *.nav *.out *.pdf || true

check: slides.pdf
	xpdf $<

LATEX_FILES = $(shell ls *.tex)

slides.pdf: $(LATEX_FILES)
	pdflatex slides
	pdflatex slides

.default: all

.phony: clean check
