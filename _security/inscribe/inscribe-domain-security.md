---
api_specs:
- filename: llms.txt
  format: yaml
  label: Inscribe Document Fraud Detection API
  slug: document-fraud-detection-api
  spec_type: OpenAPI
  url: https://docs.inscribe.ai/llms.txt
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: inscribe.ai
  spf: true
hosts:
- cert_expires: Jan  7 23:59:59 2027 GMT
  host: www.inscribe.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 06:44:40 2026 GMT
  host: docs.inscribe.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 24 23:59:59 2026 GMT
  host: api.inscribe.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Inscribe Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Inscribe, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Inscribe
provider_slug: inscribe
slug: inscribe-domain-security
source_filename: inscribe-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.inscribe.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.inscribe.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 06:44:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.inscribe.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: inscribe.ai\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inscribe/refs/heads/main/security/inscribe-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fraud Detection
- Document Verification
- Financial Services
- KYC
- KYB
- Bank Statements
- Pay Stubs
- Identity Verification
- Risk Management
- Fintech
- AI
- Machine Learning
---
