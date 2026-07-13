---
api_specs:
- filename: sandbox-banking-glyue-openapi.yml
  format: yaml
  label: Glyue Integration Gateway API
  slug: glyue
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sandbox-banking/refs/heads/main/openapi/sandbox-banking-glyue-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sandboxbanking.com
  spf: true
hosts:
- cert_expires: Jan 19 23:59:59 2027 GMT
  host: sandboxbanking.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 16:08:50 2026 GMT
  host: glyue.docs.sandboxbanking.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 01:17:44 2026 GMT
  host: mockbank.docs.sandboxbanking.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sandbox Banking Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sandbox Banking, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Sandbox Banking
provider_slug: sandbox-banking
slug: sandbox-banking-domain-security
source_filename: sandbox-banking-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sandboxbanking.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 23:59:59 2027 GMT\n  hsts: null\n- host: glyue.docs.sandboxbanking.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 16:08:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: mockbank.docs.sandboxbanking.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 01:17:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sandboxbanking.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sandbox-banking/refs/heads/main/security/sandbox-banking-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- API Integration
- Banking
- Core Banking
- Credit Unions
- Financial Services
- Fintech
- Integration Platform
- iPaaS
- Open Banking
---
