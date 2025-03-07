ASM = nasm
LD = ld

FLAGS = -felf64

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
	$(LD) $< -o $@

clean:
	rm -f *.o $(wildcard *.*)
