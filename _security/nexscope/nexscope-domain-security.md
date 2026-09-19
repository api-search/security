---
api_specs:
- filename: nexscope-openapi.json
  format: json
  label: Nexscope Ecommerce Data and Creative APIs
  slug: nexscope-ecommerce-data-and-creative-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexscope/refs/heads/main/openapi/nexscope-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nexscope.ai
  spf: true
hosts:
- cert_expires: Apr  5 23:59:59 2027 GMT
  host: www.nexscope.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr  5 23:59:59 2027 GMT
  host: api.nexscope.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Nexscope Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nexscope Ecommerce Data and Creative APIs, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Nexscope Ecommerce Data and Creative APIs
provider_slug: nexscope
slug: nexscope-domain-security
source_filename: nexscope-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nexscope.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  5 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.nexscope.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  5 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: nexscope.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nexscope/refs/heads/main/security/nexscope-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- E-Commerce
- Data
- Creative
- Artificial Intelligence
- Marketplace Intelligence
- Amazon
- TikTok
- Keyword Research
- Image-Generation
- Video Generation
- MCP
---
