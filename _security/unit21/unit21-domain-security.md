---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: unit21.ai
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: unit21.com
  spf: false
hosts:
- cert_expires: Oct  1 03:41:37 2026 GMT
  host: www.unit21.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 13:30:05 2026 GMT
  host: docs.unit21.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  3 23:59:59 2026 GMT
  host: sandbox1-api.unit21.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Unit21 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Unit21, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Unit21
provider_slug: unit21
slug: unit21-domain-security
source_filename: unit21-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.unit21.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 03:41:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.unit21.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 13:30:05 2026 GMT\n  hsts: null\n- host: sandbox1-api.unit21.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  3 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: unit21.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: unit21.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unit21/refs/heads/main/security/unit21-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fraud Detection
- AML
- Anti-Money Laundering
- Compliance
- FinTech
- Transaction Monitoring
- Risk
- SAR
- Financial Crime
- Suspicious Activity Reports
---
