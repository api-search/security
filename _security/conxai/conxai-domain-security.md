---
api_specs:
- filename: conxai-customer-openapi.json
  format: json
  label: Conxai Customer API (SiteLens)
  slug: conxai-customer-api-sitelens
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conxai/refs/heads/main/openapi/conxai-customer-openapi.json
- filename: conxai-docnostic-openapi.json
  format: json
  label: Conxai Docnostic API
  slug: conxai-docnostic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conxai/refs/heads/main/openapi/conxai-docnostic-openapi.json
- filename: conxai-firestop-openapi.json
  format: json
  label: Conxai Firestop API
  slug: conxai-firestop-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conxai/refs/heads/main/openapi/conxai-firestop-openapi.json
- filename: conxai-production-tracking-openapi.json
  format: json
  label: Conxai Production Tracking API
  slug: conxai-production-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conxai/refs/heads/main/openapi/conxai-production-tracking-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: conxai.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: readme.io
  spf: true
hosts:
- cert_expires: Sep 29 08:48:52 2026 GMT
  host: www.conxai.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 13:12:37 2026 GMT
  host: conxai.readme.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 22 23:59:59 2026 GMT
  host: customer.conxai.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Conxai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Conxai, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Conxai
provider_slug: conxai
slug: conxai-domain-security
source_filename: conxai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.conxai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 08:48:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: conxai.readme.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 13:12:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: customer.conxai.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: conxai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: readme.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/conxai/refs/heads/main/security/conxai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Construction
- AEC
- Artificial Intelligence
- Document Processing
- Computer Vision
- Agentic AI
- Machine Learning
---
