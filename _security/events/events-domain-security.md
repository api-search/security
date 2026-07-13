---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: cloudevents.io
  spf: false
- caa: []
  dmarc: false
  dnssec: false
  domain: asyncapi.com
  spf: false
hosts:
- cert_expires: Oct  3 01:48:35 2026 GMT
  host: cloudevents.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 03:28:50 2026 GMT
  host: www.asyncapi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 23:33:10 2026 GMT
  host: kafka.apache.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Events Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Events, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Events
provider_slug: events
slug: events-domain-security
source_filename: events-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cloudevents.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 01:48:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.asyncapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 03:28:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: kafka.apache.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 23:33:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cloudevents.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: asyncapi.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/events/refs/heads/main/security/events-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Events
- Event-Driven
- Event Streaming
- Messaging
- Pub Sub
- Brokers
- CloudEvents
- AsyncAPI
- Topic
---
