---
api_specs:
- filename: device-specs-api-values-api-openapi.yml
  format: yaml
  label: Device Specs API Values API
  slug: device-specs-api-values-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/device-specs-api/refs/heads/main/openapi/device-specs-api-values-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: gtgroup.dev
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: rapidapi.com
  spf: true
hosts:
- cert_expires: Oct 22 04:41:21 2026 GMT
  host: ds.gtgroup.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  3 23:59:59 2027 GMT
  host: gsmarenaparser.p.rapidapi.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Device Specs Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Device Specs API, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Device Specs API
provider_slug: device-specs-api
slug: device-specs-api-domain-security
source_filename: device-specs-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ds.gtgroup.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 04:41:21 2026 GMT\n  hsts: null\n- host: gsmarenaparser.p.rapidapi.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  3 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: gtgroup.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: rapidapi.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/device-specs-api/refs/heads/main/security/device-specs-api-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Mobile
- smartphones
- phone-specs
- chipsets
- hardware
- mobile-specs
- Devices
- rapidapi
- gsmarena
- reference-data
- Developer Tools
---
