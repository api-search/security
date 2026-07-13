---
api_specs:
- filename: climate-fieldview-platform-openapi.yml
  format: yaml
  label: Climate FieldView Platform API
  slug: fieldview-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/climate-fieldview/refs/heads/main/openapi/climate-fieldview-platform-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: climate.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: fieldview.com
  spf: false
hosts:
- cert_expires: Feb 27 23:59:59 2027 GMT
  host: climate.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 22 23:59:59 2026 GMT
  host: dev.fieldview.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 27 23:59:59 2027 GMT
  host: api.climate.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Climate Fieldview Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Climate FieldView, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Climate FieldView
provider_slug: climate-fieldview
slug: climate-fieldview-domain-security
source_filename: climate-fieldview-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: climate.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 27 23:59:59 2027 GMT\n  hsts: null\n- host: dev.fieldview.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 23:59:59 2026 GMT\n  hsts: false\n- host: api.climate.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 27 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: climate.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: fieldview.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/climate-fieldview/refs/heads/main/security/climate-fieldview-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Agriculture
- Bayer
- Crop Data
- Field Boundaries
- Harvest
- OAuth2
- Planting
- Precision Ag
---
