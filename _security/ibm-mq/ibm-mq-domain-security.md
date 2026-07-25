---
api_specs:
- filename: ibm-mq-messaging-asyncapi.yml
  format: yaml
  label: IBM MQ JMS API
  slug: ibm-mq-jms-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibm-mq/refs/heads/main/asyncapi/ibm-mq-messaging-asyncapi.yml
- filename: ibm-mq-channels-api-openapi.yml
  format: yaml
  label: IBM MQ Channels API
  slug: ibm-mq-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibm-mq/refs/heads/main/openapi/ibm-mq-channels-api-openapi.yml
- filename: ibm-mq-installations-api-openapi.yml
  format: yaml
  label: IBM MQ Installations API
  slug: ibm-mq-installations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibm-mq/refs/heads/main/openapi/ibm-mq-installations-api-openapi.yml
- filename: ibm-mq-login-api-openapi.yml
  format: yaml
  label: IBM MQ Login API
  slug: ibm-mq-login-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibm-mq/refs/heads/main/openapi/ibm-mq-login-api-openapi.yml
- filename: ibm-mq-queue-managers-api-openapi.yml
  format: yaml
  label: IBM MQ Queue Managers API
  slug: ibm-mq-queue-managers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibm-mq/refs/heads/main/openapi/ibm-mq-queue-managers-api-openapi.yml
- filename: ibm-mq-queue-messaging-api-openapi.yml
  format: yaml
  label: IBM MQ Queue Messaging API
  slug: ibm-mq-queue-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibm-mq/refs/heads/main/openapi/ibm-mq-queue-messaging-api-openapi.yml
- filename: ibm-mq-queues-api-openapi.yml
  format: yaml
  label: IBM MQ Queues API
  slug: ibm-mq-queues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibm-mq/refs/heads/main/openapi/ibm-mq-queues-api-openapi.yml
- filename: ibm-mq-subscriptions-api-openapi.yml
  format: yaml
  label: IBM MQ Subscriptions API
  slug: ibm-mq-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibm-mq/refs/heads/main/openapi/ibm-mq-subscriptions-api-openapi.yml
- filename: ibm-mq-topic-messaging-api-openapi.yml
  format: yaml
  label: IBM MQ Topic Messaging API
  slug: ibm-mq-topic-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibm-mq/refs/heads/main/openapi/ibm-mq-topic-messaging-api-openapi.yml
- filename: ibm-mq-topics-api-openapi.yml
  format: yaml
  label: IBM MQ Topics API
  slug: ibm-mq-topics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibm-mq/refs/heads/main/openapi/ibm-mq-topics-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ibm.com
  spf: true
hosts:
- cert_expires: Jan  5 23:59:59 2027 GMT
  host: www.ibm.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ibm Mq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IBM MQ, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: IBM MQ
provider_slug: ibm-mq
slug: ibm-mq-domain-security
source_filename: ibm-mq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ibm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ibm.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ibm-mq/refs/heads/main/security/ibm-mq-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Async
- Enterprise
- Integration
- Messaging
- Middleware
- Queue
---
