CC      ?= gcc
CFLAGS  ?= -O2 -pipe
PREFIX  ?= /usr
BINDIR  ?= $(PREFIX)/bin

all: hello-lunis

hello-lunis: main.o
	$(CC) $(CFLAGS) -o $@ $^

main.o: main.c
	$(CC) $(CFLAGS) -c main.c

install: all
	install -Dm00755 hello-lunis $(DESTDIR)$(BINDIR)/hello-lunis

clean:
	rm -f hello-lunis main.o
