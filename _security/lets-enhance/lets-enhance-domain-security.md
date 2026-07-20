---
api_specs:
- filename: lets-enhance-claid-openapi.json
  format: json
  label: Claid API
  slug: claid
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lets-enhance/refs/heads/main/openapi/lets-enhance-claid-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: letsenhance.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: claid.ai
  spf: true
hosts:
- cert_expires: Aug 20 14:16:08 2026 GMT
  host: letsenhance.io
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 16:47:24 2026 GMT
  host: docs.claid.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 19:07:36 2026 GMT
  host: api.claid.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lets Enhance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Let''s Enhance, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Let's Enhance
provider_slug: lets-enhance
slug: lets-enhance-domain-security
source_filename: lets-enhance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: letsenhance.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 14:16:08 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: docs.claid.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 16:47:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.claid.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 19:07:36 2026 GMT\n  hsts: null\ndomains:\n- domain: letsenhance.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: claid.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lets-enhance/refs/heads/main/security/lets-enhance-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Image Processing
- Image Enhancement
- Image Generation
- Computer Vision
- Ecommerce
- Media
- Photography
- Video Generation
---
