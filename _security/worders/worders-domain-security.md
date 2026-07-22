---
api_specs:
- filename: worders-api-openapi-original.yml
  format: yaml
  label: Worders API V1
  slug: worders-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/worders/refs/heads/main/openapi/worders-api-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: worders.net
  spf: true
hosts:
- cert_expires: Oct 13 00:45:05 2026 GMT
  host: worders.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 21 05:19:03 2026 GMT
  host: api.worders.net
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Worders Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Worders, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Worders
provider_slug: worders
slug: worders-domain-security
source_filename: worders-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: worders.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 00:45:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.worders.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 05:19:03 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: worders.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/worders/refs/heads/main/security/worders-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Applicative Saas
- Localization
- Translation
- Culturalization
- Language Services
- Invoicing
---
