---
api_specs:
- filename: leafly-menu-integration-openapi.yml
  format: yaml
  label: Leafly Menu Integration API
  slug: leafly-menu-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leafly/refs/heads/main/openapi/leafly-menu-integration-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: leafly.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: leafly.io
  spf: true
hosts:
- cert_expires: Aug 23 00:51:00 2026 GMT
  host: www.leafly.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 17 21:16:04 2026 GMT
  host: docs.leafly.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 00:51:00 2026 GMT
  host: api.leafly.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Leafly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Leafly, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Leafly
provider_slug: leafly
slug: leafly-domain-security
source_filename: leafly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.leafly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 00:51:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.leafly.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 21:16:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.leafly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 00:51:00 2026 GMT\n  hsts: null\ndomains:\n- domain: leafly.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: leafly.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leafly/refs/heads/main/security/leafly-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Cannabis
- Dispensary
- Menu Sync
- POS Integration
- Retail
- Marketplace
- Strains
- Ecommerce
---
