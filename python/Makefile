build-python-2.7:
	docker build -t "intropro/python:2.7-alpine" 2.7/alpine/

build-python-3.5:
	docker build -t "intropro/python:3.5-alpine" 3.5/alpine/

build-all: build-python-2.7 build-python-3.5
	@ echo Completed

push-python-2.7: build-python-2.7
	docker push intropro/python:2.7-alpine

push-python-3.5: build-python-3.5
	docker push intropro/python:3.5-alpine

push-all: push-python-2.7 push-python-3.5
	@ echo Completed
