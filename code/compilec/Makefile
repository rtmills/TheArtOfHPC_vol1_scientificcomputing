# -*- makefile -*-
################################################################
################################################################
####
#### This Makefile belong with the sources
#### for Introduction to High-Performance Scientific Computing
#### by Victor Eijkhout
#### copyright 2010-2021
####
#### makefile for code/compile
####
################################################################
################################################################

info ::

PROGRAM = rotate
PROGRAMS = hello rotate
LANGUAGE = C
MODE = seq
include ../../makefiles/Make.compile

include ../../makefiles/Make.run

include ../Make.rotate

##
## public copy
##
PUBLICEXTS = c
include ../../makefiles/Make.public

##
## clean rules
##
include ../../makefiles/Make.clean
clean ::
	@rm -f *.optrpt *.annot

.PHONY: example_clean
info ::
	@echo "make example_clean : remove local binaries"
example_clean ::
	@rm -f ${PROGRAMS} ${LIBS}
clean :: example_clean
	@rm -rf libs
