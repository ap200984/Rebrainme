FROM rabbitmq:3.10.7-management
COPY rabbitmq.conf /etc/rabbitmq
COPY definitions.json /etc/rabbitmq/
COPY docker_certs /etc/pki/tls/
RUN chmod 644 -R /etc/pki/tls/*
RUN rabbitmq-plugins enable rabbitmq_auth_mechanism_ssl


