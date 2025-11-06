VERSION=$(shell date +%Y%m%d)

.PHONY: build publish

build:
	docker build . -t devcontainer-python:$(VERSION)

publish:
	docker tag devcontainer-python:$(VERSION) registry.cluster:5000/devcontainer-python:$(VERSION)
	docker image push registry.cluster:5000/devcontainer-python:$(VERSION)
