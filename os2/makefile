#	MicroSoft C 6.0 makefile for
#		MicroEMACS 3.12
#		(C)Copyright 1993 by Daniel Lawrence
#		all rights reserved

# modify the following lines with the proper relative directories

OBJD = obj			# object file directory
SRCD = ..\src			# source file directory
HDIR = ..\h			# header file directory
INCD = c:\sys\c600\include	# system include directory

# options and arguments to the C compiler

CC = cl
#CFLAGS=/AL /c /FPc /Gm /Gs /I. /I$(HDIR) /I$(IDIR) /Ox /Zd
CFLAGS=/AL /c /FPc /J  /Gs /I. /I$(HDIR) /I$(IDIR) /Oas /Zpe

# list of header files

HFILES = $(HDIR)\estruct.h $(HDIR)\edef.h $(HDIR)\efunc.h $(HDIR)\epath.h $(HDIR)\ebind.h $(HDIR)\eproto.h

#list of source files

F1 = $(OBJD)\abbrev.obj $(OBJD)\basic.obj $(OBJD)\bind.obj $(OBJD)\buffer.obj
F2 = $(OBJD)\char.obj $(OBJD)\crypt.obj $(OBJD)\display.obj  $(OBJD)\dolock.obj
F3 = $(OBJD)\eval.obj $(OBJD)\exec.obj $(OBJD)\file.obj
F4 = $(OBJD)\fileio.obj $(OBJD)\os2.obj $(OBJD)\input.obj $(OBJD)\keyboard.obj
F5 = $(OBJD)\isearch.obj $(OBJD)\line.obj $(OBJD)\lock.obj
F6 = $(OBJD)\main.obj $(OBJD)\mouse.obj $(OBJD)\os2npm.obj $(OBJD)\screen.obj
F7 = $(OBJD)\random.obj $(OBJD)\region.obj $(OBJD)\search.obj $(OBJD)\replace.obj
F8 = $(OBJD)\tags.obj $(OBJD)\undo.obj $(OBJD)\window.obj $(OBJD)\word.obj

# compilation rules


$(OBJD)\abbrev.obj: $(SRCD)\abbrev.c $(HFILES)
	$(CC) $(CFLAGS) /Fo$(OBJD)\abbrev.obj $(SRCD)\abbrev.c

$(OBJD)\basic.obj: $(SRCD)\basic.c $(HFILES)
	$(CC) $(CFLAGS) /Fo$(OBJD)\basic.obj $(SRCD)\basic.c

$(OBJD)\bind.obj: $(SRCD)\bind.c $(HFILES)
	$(CC) $(CFLAGS) /Fo$(OBJD)\bind.obj $(SRCD)\bind.c

$(OBJD)\buffer.obj: $(SRCD)\buffer.c $(HFILES)
	$(CC) $(CFLAGS) /Fo$(OBJD)\buffer.obj $(SRCD)\buffer.c

$(OBJD)\char.obj: $(SRCD)\char.c $(HFILES)
	$(CC) $(CFLAGS) /Fo$(OBJD)\char.obj $(SRCD)\char.c

$(OBJD)\crypt.obj: $(SRCD)\crypt.c $(HFILES)
	$(CC) $(CFLAGS) /Fo$(OBJD)\crypt.obj $(SRCD)\crypt.c

$(OBJD)\cmdfix.obj: $(SRCD)\cmdfix.c $(HFILES)
	$(CC) $(CFLAGS) /Fo$(OBJD)\cmdfix.obj $(SRCD)\cmdfix.c

$(OBJD)\display.obj: $(SRCD)\display.c $(HFILES)
	$(CC) $(CFLAGS) /Fo$(OBJD)\display.obj $(SRCD)\display.c

$(OBJD)\dolock.obj: $(SRCD)\dolock.c $(HFILES)
	$(CC) $(CFLAGS) /Fo$(OBJD)\dolock.obj $(SRCD)\dolock.c

$(OBJD)\eval.obj: $(SRCD)\eval.c $(HFILES) $(HDIR)\evar.h
	$(CC) $(CFLAGS) /Fo$(OBJD)\eval.obj $(SRCD)\eval.c

$(OBJD)\exec.obj: $(SRCD)\exec.c $(HFILES)
	$(CC) $(CFLAGS) /Fo$(OBJD)\exec.obj $(SRCD)\exec.c

$(OBJD)\file.obj: $(SRCD)\file.c $(HFILES)
	$(CC) $(CFLAGS) /Fo$(OBJD)\file.obj $(SRCD)\file.c

$(OBJD)\fileio.obj: $(SRCD)\fileio.c $(HFILES)
	$(CC) $(CFLAGS) /Fo$(OBJD)\fileio.obj $(SRCD)\fileio.c

$(OBJD)\keyboard.obj: $(SRCD)\keyboard.c $(HFILES)
	$(CC) $(CFLAGS) /Fo$(OBJD)\keyboard.obj $(SRCD)\keyboard.c

$(OBJD)\os2.obj: $(SRCD)\os2.c $(HFILES)
	$(CC) $(CFLAGS) /Fo$(OBJD)\os2.obj $(SRCD)\os2.c

$(OBJD)\input.obj: $(SRCD)\input.c $(HFILES)
	$(CC) $(CFLAGS) /Fo$(OBJD)\input.obj $(SRCD)\input.c

$(OBJD)\isearch.obj: $(SRCD)\isearch.c $(HFILES)
	$(CC) $(CFLAGS) /Fo$(OBJD)\isearch.obj $(SRCD)\isearch.c

$(OBJD)\line.obj: $(SRCD)\line.c $(HFILES)
	$(CC) $(CFLAGS) /Fo$(OBJD)\line.obj $(SRCD)\line.c

$(OBJD)\lock.obj: $(SRCD)\lock.c $(HFILES)
	$(CC) $(CFLAGS) /Fo$(OBJD)\lock.obj $(SRCD)\lock.c

$(OBJD)\main.obj: $(SRCD)\main.c $(HFILES)
	$(CC) $(CFLAGS) /Fo$(OBJD)\main.obj $(SRCD)\main.c

$(OBJD)\mouse.obj: $(SRCD)\mouse.c $(HFILES)
	$(CC) $(CFLAGS) /Fo$(OBJD)\mouse.obj $(SRCD)\mouse.c

$(OBJD)\os2npm.obj: $(SRCD)\os2npm.c $(HFILES)
	$(CC) $(CFLAGS) /Fo$(OBJD)\os2npm.obj $(SRCD)\os2npm.c

$(OBJD)\random.obj: $(SRCD)\random.c $(HFILES)
	$(CC) $(CFLAGS) /Fo$(OBJD)\random.obj $(SRCD)\random.c

$(OBJD)\region.obj: $(SRCD)\region.c $(HFILES)
	$(CC) $(CFLAGS) /Fo$(OBJD)\region.obj $(SRCD)\region.c

$(OBJD)\search.obj: $(SRCD)\search.c $(HFILES)
	$(CC) $(CFLAGS) /Fo$(OBJD)\search.obj $(SRCD)\search.c

$(OBJD)\replace.obj: $(SRCD)\replace.c $(HFILES)
	$(CC) $(CFLAGS) /Fo$(OBJD)\replace.obj $(SRCD)\replace.c

$(OBJD)\screen.obj: $(SRCD)\screen.c $(HFILES)
	$(CC) $(CFLAGS) /Fo$(OBJD)\screen.obj $(SRCD)\screen.c

$(OBJD)\tags.obj: $(SRCD)\tags.c $(HFILES)
	$(CC) $(CFLAGS) /Fo$(OBJD)\tags.obj $(SRCD)\tags.c

$(OBJD)\undo.obj: $(SRCD)\undo.c $(HFILES)
	$(CC) $(CFLAGS) /Fo$(OBJD)\undo.obj $(SRCD)\undo.c

$(OBJD)\window.obj: $(SRCD)\window.c $(HFILES)
	$(CC) $(CFLAGS) /Fo$(OBJD)\window.obj $(SRCD)\window.c

$(OBJD)\word.obj: $(SRCD)\word.c $(HFILES)
	$(CC) $(CFLAGS) /Fo$(OBJD)\word.obj $(SRCD)\word.c

# product list

bin\emacs.exe: $(F1) $(F2) $(F3) $(F4) $(F5) $(F6) $(F7) $(F8)
	link @emacs.lnk

all:	bin\emacs.exe
