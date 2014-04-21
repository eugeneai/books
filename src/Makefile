.PHONY: all pdf ps dvi clean orig edit ru en

all: pdf

pdf: book.tex
	pdflatex book.tex

view: pdf
	evince book.pdf &

orig:
	djview ../OCR-father-1997-cuneiform.djvu &

edit:	orig pdf
	emacsclient -a emacs book.tex &

book-ru.pdf:	book-ru.tex
	lualatex $<
	#lualatex $<

ru:	book-ru.pdf

en:	book.pdf

clean:
	latexmk -C
	rm -f *.aux *.thm
