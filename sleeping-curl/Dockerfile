FROM registry.access.redhat.com/ubi8-minimal:latest

USER root

RUN microdnf update --setopt=install_weak_deps=0 --nodocs -y \
  && microdnf install --setopt=install_weak_deps=0 --nodocs -y curl \
  && microdnf clean all

USER 1001
WORKDIR /tmp

ENTRYPOINT ["sleep", "infinity"]
