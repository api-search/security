---
api_specs:
- filename: openapi.yml
  format: yaml
  label: DPLA Items API
  slug: items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dpla/refs/heads/main/openapi/openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dp.la
  spf: false
hosts:
- cert_expires: Nov 11 23:59:59 2026 GMT
  host: dp.la
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 11 23:59:59 2026 GMT
  host: pro.dp.la
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 11 23:59:59 2026 GMT
  host: api.dp.la
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dpla Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Digital Public Library of America, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Digital Public Library of America
provider_slug: dpla
slug: dpla-domain-security
source_filename: dpla-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dp.la\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 23:59:59 2026 GMT\n  hsts: null\n- host: pro.dp.la\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 23:59:59 2026 GMT\n  hsts: null\n- host: api.dp.la\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: dp.la\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dpla/refs/heads/main/security/dpla-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Cultural Heritage
- Libraries
- Archives
- Museums
- Open Data
- Metadata
- Digital Collections
- Public Domain
---
