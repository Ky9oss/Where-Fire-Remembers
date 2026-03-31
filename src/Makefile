src/memfiry: src/main.c
	$(CC) $(CFLAGS) -o $@ $<

check: all
	./src/memfiry | grep "hello.*"
	@echo "*** All TESTS PASSED"

install:
	install -d $(DESTDIR)$(bindir)
	install -m 0755 src/memfiry $(DESTDIR)$(bindir)

uninstall:
	rm -f $(DESTDIR)$(bindir)/memfiry
	-rmdir -f $(DESTDIR)$(bindir) > /dev/null 2>&1

clean:
	rm -f src/memfiry
