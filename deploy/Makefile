GIT_SHA ?= git-$(shell git rev-parse --short=12 HEAD)
K8S_NAMESPACE ?= authgear-demo

.PHONY: deploy
deploy:
	helm upgrade authgear-saml-e2e-sp ./helm --install \
		--wait --wait-for-jobs --cleanup-on-fail \
		-n $(K8S_NAMESPACE) \
		--set-string appVersion="$(GIT_SHA)"
