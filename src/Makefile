.PHONY: all pdf ps dvi clean orig

all: pdf

pdf: book.tex
	pdflatex book.tex

view: pdf
	evince book.pdf &

orig:
	djview ../father-1997.djvu &
