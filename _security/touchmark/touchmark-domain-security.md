---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: touchmark.ai
  spf: true
hosts:
- cert_expires: Dec 23 23:59:59 2026 GMT
  host: touchmark.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 26 23:59:59 2026 GMT
  host: docs.touchmark.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 23 23:59:59 2026 GMT
  host: api.touchmark.ai
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Touchmark Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Touchmark, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Touchmark
provider_slug: touchmark
slug: touchmark-domain-security
source_filename: touchmark-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: touchmark.ai\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.touchmark.ai\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.touchmark.ai\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 23 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: touchmark.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/touchmark/refs/heads/main/security/touchmark-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- AI Pricing
- Billing
- Monetization
- Evals
- Usage-Based Billing
- Quality Scoring
---
