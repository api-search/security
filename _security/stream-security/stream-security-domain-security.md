---
api_specs:
- filename: stream-security-api-openapi.json
  format: json
  label: Stream Security API
  slug: stream-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stream-security/refs/heads/main/openapi/stream-security-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: stream.security
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: streamsec.io
  spf: true
hosts:
- cert_expires: Nov 27 06:45:55 2026 GMT
  host: www.stream.security
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 13 21:07:47 2026 GMT
  host: docs.streamsec.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 21 23:59:59 2027 GMT
  host: app.streamsec.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stream Security Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stream.Security, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Stream.Security
provider_slug: stream-security
slug: stream-security-domain-security
source_filename: stream-security-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.stream.security\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 06:45:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.streamsec.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 21:07:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.streamsec.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 21 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: stream.security\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: streamsec.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stream-security/refs/heads/main/security/stream-security-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Security
- Cloud Security
- Cloud Detection and Response
- CNAPP
- Threat Detection
- Vulnerability Management
- Kubernetes
- Observability
- DevSecOps
- Artificial Intelligence
---
