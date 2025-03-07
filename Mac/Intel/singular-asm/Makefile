ASM = nasm
LD = ld

FLAGS = -f macho
LDFLAGS = -macosx_version_min 10.7 -arch x86_64

# Ensure the user provides a filename
ifeq ($(MAKECMDGOALS),)
$(error Usage: make <filename> (without extension))
endif

OBJ = $(MAKECMDGOALS).o
EXE = $(MAKECMDGOALS)

$(MAKECMDGOALS): $(EXE)

$(OBJ): $(MAKECMDGOALS).asm
	$(ASM) $(FLAGS) $< -o $@

$(EXE): $(OBJ)
	$(LD) $(LDFLAGS) $< -o $@

clean:
	rm -f *.o *
