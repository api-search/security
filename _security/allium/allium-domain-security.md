---
api_specs:
- filename: allium-openapi-original.json
  format: json
  label: Allium Realtime API
  slug: allium-realtime-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allium/refs/heads/main/openapi/allium-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: allium.so
  spf: true
hosts:
- cert_expires: Oct 11 05:59:51 2026 GMT
  host: allium.so
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 09:21:24 2026 GMT
  host: docs.allium.so
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 21 01:05:02 2026 GMT
  host: api.allium.so
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Allium Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Allium, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Allium
provider_slug: allium
slug: allium-domain-security
source_filename: allium-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: allium.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 05:59:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.allium.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 09:21:24 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.allium.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 01:05:02 2026 GMT\n  hsts: null\ndomains:\n- domain: allium.so\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allium/refs/heads/main/security/allium-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data Analytics
- Blockchain
- Crypto
- Web3
- Data Infrastructure
- Real-Time Data
- Stablecoins
- DeFi
- Machine Payments
---
