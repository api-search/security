---
api_specs:
- filename: realestateapi-openapi.yml
  format: yaml
  label: RealEstateAPI
  slug: realestateapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/realestateapi/refs/heads/main/openapi/realestateapi-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: realestateapi.com
  spf: true
hosts:
- cert_expires: Sep 23 06:46:47 2026 GMT
  host: www.realestateapi.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 11 23:38:52 2026 GMT
  host: api.realestateapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Realestateapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RealEstateAPI, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: RealEstateAPI
provider_slug: realestateapi
slug: realestateapi-domain-security
source_filename: realestateapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.realestateapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 06:46:47 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.realestateapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 11 23:38:52 2026 GMT\n  hsts: false\ndomains:\n- domain: realestateapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/realestateapi/refs/heads/main/security/realestateapi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real Estate
- Property Data
- MLS
- Valuation
- Geospatial
- Skip Tracing
- Prop-Tech
---
