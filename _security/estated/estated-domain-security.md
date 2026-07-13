---
api_specs:
- filename: estated-property-data-api-openapi.yml
  format: yaml
  label: Estated Property Data API
  slug: property-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/estated/refs/heads/main/openapi/estated-property-data-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: estated.com
  spf: true
hosts:
- cert_expires: Sep 15 01:47:51 2026 GMT
  host: estated.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 14 23:59:59 2026 GMT
  host: apis.estated.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Estated Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Estated, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Estated
provider_slug: estated
slug: estated-domain-security
source_filename: estated-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: estated.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 01:47:51 2026 GMT\n  hsts: false\n- host: apis.estated.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: estated.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/estated/refs/heads/main/security/estated-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Property Data
- Real Estate
- Property Records
- Assessor
- Parcels
- APN
- FIPS
- Deeds
- AVM
- Valuation
- Boundaries
- GIS
- Owner Of Record
- Tax Assessment
---
