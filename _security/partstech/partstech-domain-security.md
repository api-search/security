---
api_specs:
- filename: partstech-api-openapi.yml
  format: yaml
  label: PartsTech External API
  slug: partstech-external-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/partstech/refs/heads/main/openapi/partstech-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: partstech.com
  spf: true
hosts:
- cert_expires: Nov 22 23:59:59 2026 GMT
  host: partstech.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  4 23:59:59 2027 GMT
  host: api-docs.partstech.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  4 23:59:59 2027 GMT
  host: api.partstech.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Partstech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PartsTech, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: PartsTech
provider_slug: partstech
slug: partstech-domain-security
source_filename: partstech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: partstech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 23:59:59 2026 GMT\n  hsts: null\n- host: api-docs.partstech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  4 23:59:59 2027 GMT\n  hsts: null\n- host: api.partstech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  4 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: partstech.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/partstech/refs/heads/main/security/partstech-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Automotive
- Auto Parts
- Parts Procurement
- Tires
- E-Commerce
- Ordering
- Catalog
- Vehicle Data
- VIN Decoding
- Shop Management
- Punchout
- Marketplace
- Supply Chain
---
