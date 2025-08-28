VENV = .venv
PYTHON = $(VENV)/bin/python3
PIP = $(VENV)/bin/pip
.PHONY: setup clean run


run: $(VENV)/bin/activate
	$(PYTHON) app.py

$(VENV)/bin/activate: requirements.txt
	$(PYTHON) -m venv $(VENV)
	$(PIP) install -r requirements.txt


setup: requirements.txt $(VENV)/bin/activate
	pip install -r requirements.txt

## clean up __pycache__ folders
clean: 
	rm -rf __pycache__
	rm -rf $(VENV)