
all: libml libbdf


libml: usb.c color.c color.h
	gcc -shared -fPIC -std=gnu11 -Wall -lm -lusb-1.0 -o libml.so -g usb.c color.c

libbdf: bdf.c font.c font.h color.c color.h
	gcc -shared -fPIC -std=gnu11 -Wall -lm -o libbdf.so -g bdf.c font.c color.c

clean:
	rm libbdf.so libml.so
