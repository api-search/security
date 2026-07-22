---
api_specs:
- filename: stark-bank-openapi-original.yml
  format: yaml
  label: Stark Bank API
  slug: stark-bank-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stark-bank/refs/heads/main/openapi/stark-bank-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: starkbank.com
  spf: true
hosts:
- cert_expires: Sep 17 01:43:36 2026 GMT
  host: www.starkbank.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 03:24:29 2026 GMT
  host: api.starkbank.com
  hsts: true
  hsts_max_age: 3600
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 06:02:26 2026 GMT
  host: sandbox.api.starkbank.com
  hsts: true
  hsts_max_age: 3600
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stark Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stark Bank, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Stark Bank
provider_slug: stark-bank
slug: stark-bank-domain-security
source_filename: stark-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.starkbank.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 01:43:36 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.starkbank.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 03:24:29 2026 GMT\n  hsts: true\n  hsts_max_age: 3600\n- host: sandbox.api.starkbank.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 06:02:26 2026 GMT\n  hsts: true\n  hsts_max_age: 3600\ndomains:\n- domain: starkbank.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stark-bank/refs/heads/main/security/stark-bank-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Banking
- Payments
- Pix
- Boleto
- Banking as a Service
- Brazil
- Financial Services
---
