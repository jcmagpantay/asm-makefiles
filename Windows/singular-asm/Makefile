ASM = nasm
LD = ld

FLAGS = -f win32
LDFLAGS = -m i386pe

# Ensure the user provides a filename
ifeq ($(MAKECMDGOALS),)
$(error Usage: make <filename> (without extension))
endif

OBJ = $(MAKECMDGOALS).o
EXE = $(MAKECMDGOALS).exe

$(MAKECMDGOALS): $(EXE)

$(OBJ): $(MAKECMDGOALS).asm
	$(ASM) $(FLAGS) $< -o $@

$(EXE): $(OBJ)
	$(LD) $(LDFLAGS) $< -o $@

clean:
	rm -f *.o *.exe
