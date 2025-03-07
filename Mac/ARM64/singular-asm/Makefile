ASM = nasm
LD = ld

FLAGS = -f macho64
LDFLAGS = -macosx_version_min 11.0 -arch arm64

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
