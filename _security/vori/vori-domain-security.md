---
api_specs:
- filename: vori-openapi.yml
  format: yaml
  label: Vori API
  slug: vori-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vori/refs/heads/main/openapi/vori-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: vori.com
  spf: true
hosts:
- cert_expires: Sep 12 08:12:36 2026 GMT
  host: www.vori.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 11:51:06 2026 GMT
  host: api.vori.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vori Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vori, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Vori
provider_slug: vori
slug: vori-domain-security
source_filename: vori-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vori.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 08:12:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.vori.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 11:51:06 2026 GMT\n  hsts: null\ndomains:\n- domain: vori.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vori/refs/heads/main/security/vori-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Applications
- Grocery
- Point of Sale
- Retail
- Inventory
- Payments
- Commerce
---
