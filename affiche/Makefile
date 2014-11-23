.SILENT:
.PHONY:all
CC= pdflatex -output-directory=out/ $<
CIBLE=$(patsubst %.tex,out/%.pdf,$(wildcard *.tex))

all: $(CIBLE) clean
out/%.pdf:%.tex
	mkdir -p out/
	${CC} && ${CC}

.PHONY:clean
clean:
	find . -type f -iregex '.*\.\(aux\|tns\|bbl\|blg\|bmt\|flg\|idx\|log\|los\|lot\|lof\|out\|toc\|tpm\|pfg\|tpt\|mlf\|mlt\|mtc\|dvi\|ps\|nav\|snm\|vrb\|vrb\|cb\)' -delete

.PHONY:mrpropre
mrpropre: clean
	rm -rf out/





