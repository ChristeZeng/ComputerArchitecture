TEX      = xelatex
FILENAME = root
SRC      = $(FILENAME).tex
DEPS     = command.tex cover.tex body/*.tex
OBJ	     = $(FILENAME).pdf
TEXFLAG  = -shell-escape -8bit
RM	     = rm

.PHONY: clean

$(OBJ): $(SRC) $(DEPS)
	$(TEX) $(TEXFLAG) $<
	$(TEX) $(TEXFLAG) $< 

clean:
	del *.log *.aux *.toc
