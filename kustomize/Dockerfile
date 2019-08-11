FROM alpine as download

RUN wget -O kustomize https://github.com/kubernetes-sigs/kustomize/releases/download/v3.1.0/kustomize_3.1.0_linux_amd64 && \
	chmod +x kustomize

###

FROM scratch

COPY --from=download /kustomize /

ENTRYPOINT ["/kustomize"]
