default: all clean

all: altacv.cls resume.tex sidebar.tex
	pdflatex -jobname Galen-Guyer-Resume resume.tex

clean:
	rm -f *.aux
	rm -f *.bbl
	rm -f *.bcf
	rm -f *.blg
	rm -f *.fdb_latexmk
	rm -f *.fls
	rm -f *.log
	rm -f *.out
	rm -f *.run.xml
	rm -f *.synctex.gz
	rm -f *.bcf
	rm -f *.fdb_latexmk

publish:
	latexmk resume.tex -pdf -jobname=Galen-Guyer-Resume-`date +"%F_%H-%M-%S"`
	make clean
