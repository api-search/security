---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: HiveMQ REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://docs.hivemq.com/hivemq/latest/rest-api/specification/
- filename: hivemq-asyncapi.yml
  format: yaml
  label: HiveMQ MQTT over WebSocket
  slug: mqtt-websocket
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/hivemq/refs/heads/main/asyncapi/hivemq-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hivemq.com
  spf: true
hosts:
- cert_expires: Sep  2 00:53:52 2026 GMT
  host: www.hivemq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 00:13:48 2026 GMT
  host: docs.hivemq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: 127.0.0.1
  https: false
kind: domain-security
layout: security
method: probed
name: Hivemq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HiveMQ, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: HiveMQ
provider_slug: hivemq
slug: hivemq-domain-security
source_filename: hivemq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hivemq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 00:53:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.hivemq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 00:13:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: 127.0.0.1\n  https: false\ndomains:\n- domain: hivemq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hivemq/refs/heads/main/security/hivemq-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- MQTT
- IoT
- Messaging
- Message Broker
- Pub Sub
- WebSocket
---
