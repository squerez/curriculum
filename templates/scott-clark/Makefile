.PHONY: help install clean cv

help: ## Display this help message.
	@grep -E '^[a-z.A-Z_-]+:.*?## .*$$' $(MAKEFILE_LIST) | sort | awk 'BEGIN {FS = ":.*?## "}; {printf "\033[36m%-30s\033[0m %s\n", $$1, $$2}'

install: ## Installs the required packages.
	@sudo apt-get-update
	@sudo apt-get install -y texlive texlive-latex-extra

clean: ## Cleans the generated files.
	@rm -f *.aux *.log *.out *.toc *.bbl *.blg *.lof *.lot

cv: ## Generates the CV.
	@pdflatex template.tex
	@make clean
	@open template.pdf
