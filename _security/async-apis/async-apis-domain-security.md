---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: asyncapi.com
  spf: false
- caa: []
  dmarc: false
  dnssec: false
  domain: modelina.org
  spf: false
hosts:
- cert_expires: Oct  1 03:28:50 2026 GMT
  host: www.asyncapi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 03:28:50 2026 GMT
  host: studio.asyncapi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 00:08:41 2026 GMT
  host: modelina.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Async Apis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AsyncAPI, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: AsyncAPI
provider_slug: async-apis
slug: async-apis-domain-security
source_filename: async-apis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.asyncapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 03:28:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: studio.asyncapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 03:28:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: modelina.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 00:08:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: asyncapi.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: modelina.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/async-apis/refs/heads/main/security/async-apis-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- AsyncAPI
- Event-Driven Architecture
- Asynchronous APIs
- Message Brokers
- API Specifications
- Kafka
- MQTT
- AMQP
- WebSocket
- Linux Foundation
---
