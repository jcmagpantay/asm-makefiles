ASM = nasm
LD = ld

FLAGS = -felf64

%.o: %.asm
	$(ASM) $(FLAGS) $< -o $@

%: %.o
	$(LD) $< -o $@

all: 
	@echo "Usage: make <filename> (without extension)"

clean:
	rm -f *.o $(wildcard *.*)
