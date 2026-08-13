---
api_specs:
- filename: lily-ai-lilyapp-api-openapi.yml
  format: yaml
  label: LilyApp Middleware API
  slug: lilyapp-middleware-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lily-ai/refs/heads/main/openapi/lily-ai-lilyapp-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lily.ai
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: lilyai.net
  spf: true
hosts:
- cert_expires: Oct 15 02:12:47 2026 GMT
  host: lily.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 19 13:47:09 2027 GMT
  host: lilyapp-api-prd.pub.lilyai.net
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- host: lilyapp-api-stg.pub.lilyai.net
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has expired (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Lily Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lily AI, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Lily AI
provider_slug: lily-ai
slug: lily-ai-domain-security
source_filename: lily-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lily.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 02:12:47 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: lilyapp-api-prd.pub.lilyai.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 19 13:47:09 2027 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: lilyapp-api-stg.pub.lilyai.net\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has\n    expired (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: lily.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: lilyai.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lily-ai/refs/heads/main/security/lily-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Retail
- E-Commerce
- Artificial Intelligence
- Product Data
- Advertising
- Agentic Commerce
- Search
- Marketing
---
