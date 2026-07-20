---
api_specs:
- filename: corti-transcribe-asyncapi.json
  format: json
  label: Corti Speech to Text API
  slug: corti-speech-to-text-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/corti/refs/heads/main/asyncapi/corti-transcribe-asyncapi.json
- filename: corti-stream-asyncapi.json
  format: json
  label: Corti Ambient Documentation API
  slug: corti-ambient-documentation-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/corti/refs/heads/main/asyncapi/corti-stream-asyncapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: corti.ai
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: corti.app
  spf: false
hosts:
- cert_expires: Oct  4 06:01:35 2026 GMT
  host: www.corti.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 07:05:58 2026 GMT
  host: docs.corti.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 03:21:30 2026 GMT
  host: api.eu.corti.app
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Corti Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Corti, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Corti
provider_slug: corti
slug: corti-domain-security
source_filename: corti-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.corti.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 06:01:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.corti.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 07:05:58 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.eu.corti.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 03:21:30 2026 GMT\n  hsts: null\ndomains:\n- domain: corti.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: corti.app\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/corti/refs/heads/main/security/corti-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Health
- Healthcare
- Artificial Intelligence
- Speech to Text
- Medical Coding
- Clinical Documentation
- Agents
- Machine Learning
---
