---
api_specs:
- filename: otter-public-api-openapi.yml
  format: yaml
  label: Otter Public API
  slug: public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/otter/refs/heads/main/openapi/otter-public-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tryotter.com
  spf: true
hosts:
- cert_expires: Sep  4 00:52:35 2026 GMT
  host: www.tryotter.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 05:47:33 2026 GMT
  host: developer-guides.tryotter.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Otter Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Otter, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Otter
provider_slug: otter
slug: otter-domain-security
source_filename: otter-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tryotter.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 00:52:35 2026 GMT\n  hsts: false\n- host: developer-guides.tryotter.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 05:47:33 2026 GMT\n  hsts: null\ndomains:\n- domain: tryotter.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/otter/refs/heads/main/security/otter-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Restaurant
- Order Management
- Delivery
- Online Ordering
- Menu Management
- Analytics
---
