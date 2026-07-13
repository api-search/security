---
api_specs:
- filename: messari-openapi.yml
  format: yaml
  label: Messari REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messari/refs/heads/main/openapi/messari-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: messari.io
  spf: true
hosts:
- cert_expires: Sep 25 05:09:19 2026 GMT
  host: messari.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 23:59:59 2026 GMT
  host: data.messari.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Messari Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Messari, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Messari
provider_slug: messari
slug: messari-domain-security
source_filename: messari-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: messari.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 05:09:19 2026 GMT\n  hsts: null\n- host: data.messari.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: messari.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/messari/refs/heads/main/security/messari-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Web3
- Crypto
- Research
- Analytics
- Asset Data
- Fundamentals
- News
- Token Unlocks
---
