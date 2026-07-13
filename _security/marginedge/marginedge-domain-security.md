---
api_specs:
- filename: marginedge-openapi.yml
  format: yaml
  label: MarginEdge Public API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marginedge/refs/heads/main/openapi/marginedge-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: marginedge.com
  spf: true
hosts:
- cert_expires: Aug 26 04:07:34 2026 GMT
  host: www.marginedge.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 17 23:59:59 2026 GMT
  host: developer.marginedge.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 17 23:59:59 2026 GMT
  host: api.marginedge.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Marginedge Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MarginEdge, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: MarginEdge
provider_slug: marginedge
slug: marginedge-domain-security
source_filename: marginedge-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.marginedge.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 04:07:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.marginedge.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 23:59:59 2026 GMT\n  hsts: false\n- host: api.marginedge.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: marginedge.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/marginedge/refs/heads/main/security/marginedge-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Restaurant
- Back Office
- Invoices
- Inventory
- Accounting
- Reporting
---
