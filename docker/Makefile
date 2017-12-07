.PHONY:

REPOSITORY=017940900017.dkr.ecr.us-west-2.amazonaws.com/haskell

build-%:
	docker build -t $(REPOSITORY):$* $*

publish-%: build-%
	docker push $(REPOSITORY):$*
