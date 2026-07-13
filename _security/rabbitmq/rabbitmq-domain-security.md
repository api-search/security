---
api_specs:
- filename: rabbitmq-management.yml
  format: yaml
  label: RabbitMQ Management HTTP API
  slug: rabbitmq-management-http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rabbitmq/refs/heads/main/openapi/rabbitmq-management.yml
- filename: rabbitmq-messaging.yml
  format: yaml
  label: RabbitMQ AMQP Messaging API
  slug: rabbitmq-amqp-messaging-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/rabbitmq/refs/heads/main/asyncapi/rabbitmq-messaging.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: rabbitmq.com
  spf: true
hosts:
- cert_expires: Sep 15 16:09:47 2026 GMT
  host: www.rabbitmq.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rabbitmq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RabbitMQ, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: RabbitMQ
provider_slug: rabbitmq
slug: rabbitmq-domain-security
source_filename: rabbitmq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rabbitmq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 16:09:47 2026 GMT\n  hsts: false\ndomains:\n- domain: rabbitmq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rabbitmq/refs/heads/main/security/rabbitmq-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AMQP
- Distributed Systems
- Event Streaming
- Message Broker
- Messaging
- Queue
---
