---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: datasutram.ai
  spf: false
hosts:
- cert_expires: Sep  8 09:24:01 2026 GMT
  host: datasutram.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Data Sutram Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Data Sutram, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Data Sutram
provider_slug: data-sutram
slug: data-sutram-domain-security
source_filename: data-sutram-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: datasutram.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 09:24:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: datasutram.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/data-sutram/refs/heads/main/security/data-sutram-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fraud Detection
- Identity Verification
- Financial Services
- Data Intelligence
- Address Verification
- Credit Risk
- Collections
- Artificial Intelligence
- India
---
