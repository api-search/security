---
api_specs:
- filename: lightbox-zoning-api-openapi.yml
  format: yaml
  label: LightBox Zoning API
  slug: lightbox-zoning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightbox-zoning-api/refs/heads/main/openapi/lightbox-zoning-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lightboxre.com
  spf: true
hosts:
- cert_expires: Jan 23 23:59:59 2027 GMT
  host: developer.lightboxre.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 21 23:59:59 2027 GMT
  host: api.lightboxre.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lightbox Zoning Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LightBox Zoning API, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: LightBox Zoning API
provider_slug: lightbox-zoning-api
slug: lightbox-zoning-api-domain-security
source_filename: lightbox-zoning-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.lightboxre.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.lightboxre.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 21 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: lightboxre.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lightbox-zoning-api/refs/heads/main/security/lightbox-zoning-api-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Zoning
- Real Estate
- CRE
- Property
- Parcels
- Geospatial
- Land Use
---
