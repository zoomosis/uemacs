#	Turbo C 2.0/Rational System's DOS16M makefile for
#		MicroEMACS 4.00
#		(C)Copyright 1996 by Daniel Lawrence
#		all rights reserved

# modify the following lines with the proper relative directories

OBJD = obj			# object file directory
SRCD = ..\..\src		# source file directory
HDIR = ..\..\h			# header file directory
INCD = c:\sys\turbo\include	# system include directory
RAT = c:\sys\dos16m		# location of the Rational DOS/16M package

# options and arguments to the C compiler

CC = tcc

#These options or with debugging on!
CFLAGS=-c -d -I. -I$(HDIR) -I$(INCD) -K -ml -N- -n$(OBJD) -O -r -v -w-par -y -Z -1

#These options are production (no debugging)
#CFLAGS=-c -d -I. -I$(HDIR) -I$(INCD) -K -ml -N- -n$(OBJD) -O -r -w-par -Z 

# list of header files

HFILES = ..\..\h\estruct.h ..\..\h\edef.h ..\..\h\efunc.h ..\..\h\epath.h ..\..\h\ebind.h ..\..\h\eproto.h

#list of source files

F1 = $(OBJD)\abbrev.obj $(OBJD)\basic.obj $(OBJD)\bind.obj $(OBJD)\buffer.obj
F2 = $(OBJD)\char.obj $(OBJD)\crypt.obj $(OBJD)\display.obj
F3 = $(OBJD)\eval.obj $(OBJD)\exec.obj $(OBJD)\file.obj $(OBJD)\tags.obj
F4 = $(OBJD)\fileio.obj $(OBJD)\ibmpc.obj $(OBJD)\input.obj $(OBJD)\isearch.obj
F5 = $(OBJD)\keyboard.obj $(OBJD)\line.obj $(OBJD)\lock.obj $(OBJD)\dolock.obj
F6 = $(OBJD)\main.obj $(OBJD)\mouse.obj $(OBJD)\msdos.obj $(OBJD)\screen.obj
F7 = $(OBJD)\random.obj $(OBJD)\region.obj $(OBJD)\search.obj $(OBJD)\replace.obj
F8 = $(OBJD)\undo.obj $(OBJD)\window.obj $(OBJD)\word.obj

# product list

all:	bin\emacs.exe

bin\emacs.exp: $(F1) $(F2) $(F3) $(F4) $(F5) $(F6) $(F7) $(F8)
	$(RAT)\glu\glu @emacs.glu

bin\emacs.exe: bin\emacs.exp
	$(RAT)\tools\splice bin\emacs.exe bin\emacs.exp $(RAT)\tools\loader
#	$(RAT)\tools\splice bin\emacs.exe $(RAT)\packages\mouse33 bin\emacs.exp $(RAT)\tools\loader

# compilation rules

$(OBJD)\abbrev.obj: $(SRCD)\abbrev.c $(HFILES)
	$(CC) $(CFLAGS) -o$(OBJD)\$&.obj $(SRCD)\$&.c
$(OBJD)\basic.obj: $(SRCD)\basic.c $(HFILES)
	$(CC) $(CFLAGS) -o$(OBJD)\$&.obj $(SRCD)\$&.c
$(OBJD)\bind.obj: $(SRCD)\bind.c $(HFILES)
	$(CC) $(CFLAGS) -o$(OBJD)\$&.obj $(SRCD)\$&.c
$(OBJD)\buffer.obj: $(SRCD)\buffer.c $(HFILES)
	$(CC) $(CFLAGS) -o$(OBJD)\$&.obj $(SRCD)\$&.c
$(OBJD)\char.obj: $(SRCD)\char.c $(HFILES)
	$(CC) $(CFLAGS) -o$(OBJD)\$&.obj $(SRCD)\$&.c
$(OBJD)\crypt.obj: $(SRCD)\crypt.c $(HFILES)
	$(CC) $(CFLAGS) -o$(OBJD)\$&.obj $(SRCD)\$&.c
$(OBJD)\display.obj: $(SRCD)\display.c $(HFILES)
	$(CC) $(CFLAGS) -o$(OBJD)\$&.obj $(SRCD)\$&.c
$(OBJD)\eval.obj: $(SRCD)\eval.c $(HFILES) $(HDIR)\evar.h
	$(CC) $(CFLAGS) -o$(OBJD)\$&.obj $(SRCD)\$&.c
$(OBJD)\exec.obj: $(SRCD)\exec.c $(HFILES)
	$(CC) $(CFLAGS) -o$(OBJD)\$&.obj $(SRCD)\$&.c
$(OBJD)\file.obj: $(SRCD)\file.c $(HFILES)
	$(CC) $(CFLAGS) -o$(OBJD)\$&.obj $(SRCD)\$&.c
$(OBJD)\fileio.obj: $(SRCD)\fileio.c $(HFILES)
	$(CC) $(CFLAGS) -o$(OBJD)\$&.obj $(SRCD)\$&.c
$(OBJD)\hp150.obj: $(SRCD)\hp150.c $(HFILES)
	$(CC) $(CFLAGS) -o$(OBJD)\$&.obj $(SRCD)\$&.c
$(OBJD)\ibmpc.obj: $(SRCD)\ibmpc.c $(HFILES)
	$(CC) $(CFLAGS) -o$(OBJD)\$&.obj $(SRCD)\$&.c
$(OBJD)\input.obj: $(SRCD)\input.c $(HFILES)
	$(CC) $(CFLAGS) -o$(OBJD)\$&.obj $(SRCD)\$&.c
$(OBJD)\isearch.obj: $(SRCD)\isearch.c $(HFILES)
	$(CC) $(CFLAGS) -o$(OBJD)\$&.obj $(SRCD)\$&.c
$(OBJD)\keyboard.obj: $(SRCD)\keyboard.c $(HFILES)
	$(CC) $(CFLAGS) -o$(OBJD)\$&.obj $(SRCD)\$&.c
$(OBJD)\line.obj: $(SRCD)\line.c $(HFILES)
	$(CC) $(CFLAGS) -o$(OBJD)\$&.obj $(SRCD)\$&.c
$(OBJD)\lock.obj: $(SRCD)\lock.c $(HFILES)
	$(CC) $(CFLAGS) -o$(OBJD)\$&.obj $(SRCD)\$&.c
$(OBJD)\dolock.obj: $(SRCD)\dolock.c $(HFILES)
	$(CC) $(CFLAGS) -o$(OBJD)\$&.obj $(SRCD)\$&.c
$(OBJD)\main.obj: $(SRCD)\main.c $(HFILES)
	$(CC) $(CFLAGS) -o$(OBJD)\$&.obj $(SRCD)\$&.c
$(OBJD)\mouse.obj: $(SRCD)\mouse.c $(HFILES)
	$(CC) $(CFLAGS) -o$(OBJD)\$&.obj $(SRCD)\$&.c
$(OBJD)\msdos.obj: $(SRCD)\msdos.c $(HFILES)
	$(CC) $(CFLAGS) -o$(OBJD)\$&.obj $(SRCD)\$&.c
$(OBJD)\random.obj: $(SRCD)\random.c $(HFILES)
	$(CC) $(CFLAGS) -o$(OBJD)\$&.obj $(SRCD)\$&.c
$(OBJD)\region.obj: $(SRCD)\region.c $(HFILES)
	$(CC) $(CFLAGS) -o$(OBJD)\$&.obj $(SRCD)\$&.c
$(OBJD)\search.obj: $(SRCD)\search.c $(HFILES)
	$(CC) $(CFLAGS) -o$(OBJD)\$&.obj $(SRCD)\$&.c
$(OBJD)\replace.obj: $(SRCD)\replace.c $(HFILES)
	$(CC) $(CFLAGS) -o$(OBJD)\$&.obj $(SRCD)\$&.c
$(OBJD)\screen.obj: $(SRCD)\screen.c $(HFILES)
	$(CC) $(CFLAGS) -o$(OBJD)\$&.obj $(SRCD)\$&.c
$(OBJD)\tags.obj: $(SRCD)\tags.c $(HFILES)
	$(CC) $(CFLAGS) -o$(OBJD)\$&.obj $(SRCD)\$&.c
$(OBJD)\undo.obj: $(SRCD)\undo.c $(HFILES)
	$(CC) $(CFLAGS) -o$(OBJD)\$&.obj $(SRCD)\$&.c
$(OBJD)\window.obj: $(SRCD)\window.c $(HFILES)
	$(CC) $(CFLAGS) -o$(OBJD)\$&.obj $(SRCD)\$&.c
$(OBJD)\word.obj: $(SRCD)\word.c $(HFILES)
	$(CC) $(CFLAGS) -o$(OBJD)\$&.obj $(SRCD)\$&.c
