# Makefile to use knitrBootstrap for package vignettes
# Modified from https://hedgehog.fhcrc.org/bioconductor/trunk/madman/Rpacks/ggbio/vignettes/Makefile
# and
# https://hedgehog.fhcrc.org/bioconductor/trunk/madman/Rpacks/BiocCheck/vignettes/Makefile

all:
	cp realVignettes/*.Rmd .
	"$(R_HOME)/bin$(R_ARCH_BIN)/Rscript" -e "library(methods); library(knitrBootstrap); knitrBoostrapFlag <- packageVersion('knitrBootstrap') < '1.0.0'; if(knitrBoostrapFlag) knit_bootstrap('derfinderHelper.Rmd', chooser=c('boot', 'code'), show_code=TRUE) else {library(rmarkdown); render('derfinderHelper.Rmd', bootstrap_document(theme.chooser=TRUE, highlight.chooser=TRUE))}"

clean:
	rm -f *.bib *.md
	cp fakeVignettes/*.Rmd .
