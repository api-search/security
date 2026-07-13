---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: TagoIO REST API
  slug: tago-io-rest-api
  spec_type: OpenAPI
  url: https://api.docs.tago.io/
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: tago.io
  spf: true
hosts:
- cert_expires: Oct  4 23:59:59 2026 GMT
  host: tago.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 23:59:59 2026 GMT
  host: docs.tago.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  3 23:59:59 2027 GMT
  host: api.us-e1.tago.io
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Tago Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TagoIO, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: TagoIO
provider_slug: tago-io
slug: tago-io-domain-security
source_filename: tago-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tago.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 23:59:59 2026 GMT\n  hsts: false\n- host: docs.tago.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 23:59:59 2026 GMT\n  hsts: false\n- host: api.us-e1.tago.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  3 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: tago.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tago-io/refs/heads/main/security/tago-io-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- IoT
- Internet of Things
- Devices
- Data Storage
- Dashboards
- Analysis
- Alerts
- MQTT
- Telemetry
---
