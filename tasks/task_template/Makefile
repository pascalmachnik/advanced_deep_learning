all: build/report.pdf

build/report.pdf: FORCE | build
	TEXINPUTS=../../latex_config: \
	BIBINPUTS=../../latex_config: \
	max_print_line=1048576 \
	latexmk \
	  --lualatex \
	  --output-directory=build \
	  --interaction=nonstopmode \
	  --halt-on-error \
	report.tex

preview: FORCE | build
	TEXINPUTS=../../latex_config: \
	BIBINPUTS=../../latex_config: \
	max_print_line=1048576 \
	latexmk \
	   -pvc \
	  --lualatex \
	  --output-directory=build \
	  --interaction=nonstopmode \
	  --halt-on-error \
	report.tex

build:
	mkdir -p build

clean:
	rm -rf build

FORCE:

.PHONY: all clean
