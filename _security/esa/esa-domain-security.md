---
api_specs:
- filename: esa-copernicus-stac-openapi.json
  format: json
  label: Copernicus Data Space STAC Catalogue API
  slug: copernicus-stac
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/esa/refs/heads/main/openapi/esa-copernicus-stac-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: esa.int
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: copernicus.eu
  spf: true
hosts:
- cert_expires: Nov  3 23:59:59 2026 GMT
  host: www.esa.int
  hsts: true
  hsts_max_age: 15552001
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  9 23:59:59 2027 GMT
  host: documentation.dataspace.copernicus.eu
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  9 23:59:59 2027 GMT
  host: catalogue.dataspace.copernicus.eu
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Esa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for European Space Agency (ESA), probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: European Space Agency (ESA)
provider_slug: esa
slug: esa-domain-security
source_filename: esa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.esa.int\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  3 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552001\n- host: documentation.dataspace.copernicus.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 23:59:59 2027 GMT\n  hsts: false\n- host: catalogue.dataspace.copernicus.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: esa.int\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: copernicus.eu\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/esa/refs/heads/main/security/esa-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Earth Observation
- Copernicus
- Sentinel
- Space Weather
- Astronomy
- Satellite Data
- Climate
- Geospatial
- STAC
- OData
---
