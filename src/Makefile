.PHONY: all pdf ps dvi clean orig edit

all: pdf

pdf: book.tex
	pdflatex book.tex

view: pdf
	evince book.pdf &

orig:
	djview ../father-1997.djvu &

edit:	orig pdf
	emacs book.tex &
