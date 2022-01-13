# Public Domain

all:
	${CC} ${CFLAGS} ${LDFLAGS} -o truncate truncate.c

install:
	install -c -S -s -m 555 truncate ${PREFIX}/bin
	install -c -m 444 truncate.1 ${PREFIX}/man/man1

test:
	@echo No tests
