NAME=860

$(NAME).agc.bin: $(NAME).agc
	yaYUL $< > $(NAME).lst

run: $(NAME).agc.bin
	yaDSKY2 &
	yaAGC --port=19797 $<

clean:
	rm -f *~ *.lst *.bin *.symtab core

.PHONY: run clean
