# This makefile is based on the advice given on
# https://learnbyexample.github.io/tutorial/ebook-generation/customizing-pandoc/

# for details, see
# https://tex.stackexchange.com/questions/234786/how-to-set-a-font-family-with-pandoc
PANDOC_VARS=-V linkcolor:blue \
    -V geometry:a4paper \
    -V geometry:margin=2cm \
	-V fontsize=11

# https://tex.stackexchange.com/questions/21736/using-xelatex-instead-of-pdflatex
PDF_ENGINE?=pdflatex

MD_FILES=$(wildcard [0-9]*md)
SORTED_MDS=$(sort $(MD_FILES))


all : ecml2021_teachingML_workshop.pdf

draft : ecml2021_teachingML_workshop.pdf

ecml2021_teachingML_workshop.md : $(SORTED_MDS)
	@cat $(SORTED_MDS) > $@
	@cat references.md >> $@

%.pdf : %.md
	@pandoc -o $@ -f gfm $(PANDOC_VARS) --pdf-engine=${PDF_ENGINE} $<

variables :
	@pandoc -D latex
