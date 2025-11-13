CC ?= gcc
CFLAGS ?= -O2 -pipe -Wall
PREFIX ?= /usr

all: hello-lunis

hello-lunis: ./src/hello.c
	$(CC) $(CFLAGS) -o $@ $<

install: all
	install -Dm755 hello-lunis $(DESTDIR)$(PREFIX)/bin/hello-lunis
