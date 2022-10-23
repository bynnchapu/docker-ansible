FROM amazon/aws-cli as awscli

FROM amazonlinux:2
RUN amazon-linux-extras install -y ansible2
RUN yum install -y less groff \
    && yum clean all
COPY --from=awscli /usr/local/aws-cli/ /usr/local/aws-cli/
COPY --from=awscli /usr/local/bin/ /usr/local/bin/