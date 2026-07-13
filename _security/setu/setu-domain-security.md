---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: setu.co
  spf: true
hosts:
- cert_expires: Jan  1 23:59:59 2027 GMT
  host: setu.co
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan 22 23:59:59 2027 GMT
  host: docs.setu.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec  3 23:59:59 2026 GMT
  host: bridge.setu.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Setu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Setu, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Setu
provider_slug: setu
slug: setu-domain-security
source_filename: setu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: setu.co\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  1 23:59:59 2027 GMT\n  hsts: false\n- host: docs.setu.co\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 22 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: bridge.setu.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: setu.co\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/setu/refs/heads/main/security/setu-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Embedded Finance
- APIs
- UPI
- BBPS
- Account Aggregator
- KYC
- eSign
- India
- Fintech
---
