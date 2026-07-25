---
api_specs:
- filename: rabbitmq-messaging.yml
  format: yaml
  label: RabbitMQ AMQP Messaging API
  slug: rabbitmq-amqp-messaging-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/rabbitmq/refs/heads/main/asyncapi/rabbitmq-messaging.yml
- filename: rabbitmq-bindings-api-openapi.yml
  format: yaml
  label: RabbitMQ Bindings API
  slug: rabbitmq-bindings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rabbitmq/refs/heads/main/openapi/rabbitmq-bindings-api-openapi.yml
- filename: rabbitmq-channels-api-openapi.yml
  format: yaml
  label: RabbitMQ Channels API
  slug: rabbitmq-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rabbitmq/refs/heads/main/openapi/rabbitmq-channels-api-openapi.yml
- filename: rabbitmq-connections-api-openapi.yml
  format: yaml
  label: RabbitMQ Connections API
  slug: rabbitmq-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rabbitmq/refs/heads/main/openapi/rabbitmq-connections-api-openapi.yml
- filename: rabbitmq-definitions-api-openapi.yml
  format: yaml
  label: RabbitMQ Definitions API
  slug: rabbitmq-definitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rabbitmq/refs/heads/main/openapi/rabbitmq-definitions-api-openapi.yml
- filename: rabbitmq-exchanges-api-openapi.yml
  format: yaml
  label: RabbitMQ Exchanges API
  slug: rabbitmq-exchanges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rabbitmq/refs/heads/main/openapi/rabbitmq-exchanges-api-openapi.yml
- filename: rabbitmq-health-api-openapi.yml
  format: yaml
  label: RabbitMQ Health API
  slug: rabbitmq-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rabbitmq/refs/heads/main/openapi/rabbitmq-health-api-openapi.yml
- filename: rabbitmq-nodes-api-openapi.yml
  format: yaml
  label: RabbitMQ Nodes API
  slug: rabbitmq-nodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rabbitmq/refs/heads/main/openapi/rabbitmq-nodes-api-openapi.yml
- filename: rabbitmq-overview-api-openapi.yml
  format: yaml
  label: RabbitMQ Overview API
  slug: rabbitmq-overview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rabbitmq/refs/heads/main/openapi/rabbitmq-overview-api-openapi.yml
- filename: rabbitmq-permissions-api-openapi.yml
  format: yaml
  label: RabbitMQ Permissions API
  slug: rabbitmq-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rabbitmq/refs/heads/main/openapi/rabbitmq-permissions-api-openapi.yml
- filename: rabbitmq-policies-api-openapi.yml
  format: yaml
  label: RabbitMQ Policies API
  slug: rabbitmq-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rabbitmq/refs/heads/main/openapi/rabbitmq-policies-api-openapi.yml
- filename: rabbitmq-queues-api-openapi.yml
  format: yaml
  label: RabbitMQ Queues API
  slug: rabbitmq-queues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rabbitmq/refs/heads/main/openapi/rabbitmq-queues-api-openapi.yml
- filename: rabbitmq-users-api-openapi.yml
  format: yaml
  label: RabbitMQ Users API
  slug: rabbitmq-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rabbitmq/refs/heads/main/openapi/rabbitmq-users-api-openapi.yml
- filename: rabbitmq-virtual-hosts-api-openapi.yml
  format: yaml
  label: RabbitMQ Virtual Hosts API
  slug: rabbitmq-virtual-hosts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rabbitmq/refs/heads/main/openapi/rabbitmq-virtual-hosts-api-openapi.yml
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
