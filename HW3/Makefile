PYTHON = python
SH = /bin/sh
VIEWER = more
SERVER = server.py
SUDO = sudo
PYDOC = pydoc server logging
ARGS = server.log 2123

TESTSCRIPT=tests/test.sh

.PHONY: run view clean test

run:
	$(PYTHON) $(SERVER) $(ARGS)
view:
	$(VIEWER) $(SERVER) $(SERVER) README
server:
	$(PYTHON) $(SERVER) $(ARGS)
docs:
	$(PYDOC)

test:
	$(SH) $(TESTSCRIPT)

clean:
	@echo "Removing .pyc and log files"
	@rm *.pyc



