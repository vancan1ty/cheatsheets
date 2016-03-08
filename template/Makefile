TeX	=	pdftex -output-directory output
CAT	=	pdfunite.exe #CB note I changed how CAT works check the code.

PAGES	= t4.pdf 
cheat:	cheat.pdf

cheat.pdf: $(PAGES)
	$(CAT) output/$(PAGES) output/cheat.pdf

cheat.tex: ../core/psfig.tex ../core/stables.tex ../core/macros.tex

t4.pdf:	t4.tex 
	$(TeX) t4.tex

clean:
	rm -f output/* 

rebuild: $(FILE)

view:
	AcroRd32.exe /n $(RFILE)

reopen: rebuild
	AcroRd32.exe /n output/$(FILE)

#depend:
#	./bin/makedepend t?.tex t10.tex

# DO NOT DELETE THIS LINE -- make depend depends on it.

t4.pdf:  cheat.tex content_tex/trig1.tex content_tex/matrix.tex content_tex/trig2.tex content_tex/hyper.tex content_tex/table.tex content_tex/quote4.tex
