FROM centos:7
MAINTAINER <muyuefei158@gmail.com>
COPY . /code
WORKDIR /code
ARG account
ARG password
ARG command
ENV ACCOUNT ${account}
ENV PASSWORD ${password}
ENV COMMAND ${command}
RUN mv .gotty ~/.gotty
CMD ./gotty -w -c "${ACCOUNT}:${PASSWORD}" --permit-arguments ${COMMAND}
