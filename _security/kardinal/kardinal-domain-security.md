---
api_specs:
- filename: kardinal-aro-openapi-original.yml
  format: yaml
  label: Kardinal ARO API
  slug: aro
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kardinal/refs/heads/main/openapi/kardinal-aro-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kardinal.ai
  spf: true
hosts:
- cert_expires: Sep 13 04:39:39 2026 GMT
  host: kardinal.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 12:03:11 2026 GMT
  host: developers.kardinal.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 19 17:39:28 2026 GMT
  host: app.kardinal.ai
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kardinal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kardinal, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kardinal
provider_slug: kardinal
slug: kardinal-domain-security
source_filename: kardinal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kardinal.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 04:39:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.kardinal.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 12:03:11 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.kardinal.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 17:39:28 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\ndomains:\n- domain: kardinal.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kardinal/refs/heads/main/security/kardinal-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- SaaS
- Route Optimization
- Vehicle Routing
- Last Mile Delivery
- Logistics
- Supply Chain
- Transportation
- Fleet Management
- Optimization
---
