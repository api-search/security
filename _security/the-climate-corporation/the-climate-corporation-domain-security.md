---
api_specs:
- filename: the-climate-corporation-platform-openapi-original.yml
  format: yaml
  label: Climate FieldView Platform API
  slug: climate-fieldview-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-climate-corporation/refs/heads/main/openapi/the-climate-corporation-platform-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: climate.com
  spf: true
hosts:
- cert_expires: Feb 27 23:59:59 2027 GMT
  host: platform.climate.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: The Climate Corporation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Climate Corporation, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: The Climate Corporation
provider_slug: the-climate-corporation
slug: the-climate-corporation-domain-security
source_filename: the-climate-corporation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: platform.climate.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 27 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: climate.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-climate-corporation/refs/heads/main/security/the-climate-corporation-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Climate
- Agriculture
- AgTech
- Digital Agriculture
- Farm Management
- Geospatial
- APIs
---
