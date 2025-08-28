## Makefile for project tasks


## tells Make that 'help' is not a file target
.PHONY: help 
help: 	## Show this help message.
		@echo "Available commands:"
		@grep -E '^[a-zA-Z_-]+:.*?## .*$$' $(MAKEFILE_LIST) | sort | awk 'BEGIN {FS = ":.*?## "}; {printf "  \033[36m%-15s\033[0m %s\n", $$1, $$2}'
.DEFAULT_GOAL := help
