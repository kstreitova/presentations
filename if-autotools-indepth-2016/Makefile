ELEMENTNAME=if-autotools-indepth-2016

all: dot doc clean

dot:
	for dotfile in *.dot; do \
		dot -Tpng $$dotfile > $${dotfile/.dot/.png} ; \
	done

doc: dot $(ELEMENTNAME).tex 
	texi2pdf $(ELEMENTNAME).tex

clean:
	rm -rf *.{aux,toc,log,out,snm,nav,lot,lol,lof}
	rm -rf *~
