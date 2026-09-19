---
api_specs:
- filename: advanceai-authentication-api-openapi.yml
  format: yaml
  label: ADVANCE.AI Authentication API
  slug: advanceai-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/advanceai/refs/heads/main/openapi/advanceai-authentication-api-openapi.yml
- filename: advanceai-document-verification-api-openapi.yml
  format: yaml
  label: ADVANCE.AI Document Verification API
  slug: advanceai-document-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/advanceai/refs/heads/main/openapi/advanceai-document-verification-api-openapi.yml
- filename: advanceai-face-comparison-api-openapi.yml
  format: yaml
  label: ADVANCE.AI Face Comparison API
  slug: advanceai-face-comparison-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/advanceai/refs/heads/main/openapi/advanceai-face-comparison-api-openapi.yml
- filename: advanceai-liveness-detection-api-openapi.yml
  format: yaml
  label: ADVANCE.AI Liveness Detection API
  slug: advanceai-liveness-detection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/advanceai/refs/heads/main/openapi/advanceai-liveness-detection-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: advance.ai
  spf: true
hosts:
- cert_expires: Oct 20 01:35:17 2026 GMT
  host: advance.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 23:59:59 2026 GMT
  host: doc.advance.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 20 23:59:59 2027 GMT
  host: api.advance.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Advanceai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ADVANCE.AI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ADVANCE.AI
provider_slug: advanceai
slug: advanceai-domain-security
source_filename: advanceai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: advance.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 01:35:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: doc.advance.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.advance.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 20 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: advance.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/advanceai/refs/heads/main/security/advanceai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Identity Verification
- KYC
- KYB
- AML
- Fraud Prevention
- Face Recognition
- Liveness Detection
- OCR
- Document Verification
- Risk Management
- Artificial Intelligence
- Fintech
- Singapore
---
