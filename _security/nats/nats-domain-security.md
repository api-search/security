---
api_specs:
- filename: nats-monitoring-api-openapi.yml
  format: yaml
  label: NATS Monitoring API
  slug: nats-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nats/refs/heads/main/properties/nats-monitoring-api-openapi.yml
- filename: nats-messaging-asyncapi.yml
  format: yaml
  label: NATS Messaging API
  slug: nats-messaging-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/nats/refs/heads/main/properties/nats-messaging-asyncapi.yml
- filename: nats-jetstream-api-asyncapi.yml
  format: yaml
  label: NATS JetStream Management API
  slug: nats-jetstream-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/nats/refs/heads/main/properties/nats-jetstream-api-asyncapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nats.io
  spf: true
hosts:
- cert_expires: Aug 21 00:33:44 2026 GMT
  host: nats.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 04:30:59 2026 GMT
  host: docs.nats.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nats Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NATS, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: NATS
provider_slug: nats
slug: nats-domain-security
source_filename: nats-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nats.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 00:33:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.nats.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 04:30:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nats.io\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nats/refs/heads/main/security/nats-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud Native
- IoT
- Message Broker
- Microservices
- Pub Sub
---
