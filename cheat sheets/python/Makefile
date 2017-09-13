MAIN=python

all: $(MAIN).pdf

$(MAIN).pdf: $(MAIN).tex Makefile
	latexmk -pdf -pdflatex="pdflatex --shell-escape %O %S" $(MAIN)

clean:
	rm -rf _minted-$(MAIN)
	rm -f $(MAIN).aux $(MAIN).bbl $(MAIN).blg $(MAIN).dvi $(MAIN).fdb_latexmk \
		$(MAIN).fls $(MAIN).log $(MAIN).nav $(MAIN).out $(MAIN).snm \
		$(MAIN).synctex.gz $(MAIN).toc $(MAIN).vrb missfont.log .DS_Store

.PHONY: clean all

