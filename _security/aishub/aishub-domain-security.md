---
api_specs:
- filename: aishub-openapi.yml
  format: yaml
  label: AISHub Vessel Positions API
  slug: aishub-vessel-positions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aishub/refs/heads/main/openapi/aishub-openapi.yml
- filename: aishub-openapi.yml
  format: yaml
  label: AISHub Stations API
  slug: aishub-stations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aishub/refs/heads/main/openapi/aishub-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: aishub.net
  spf: true
hosts:
- cert_expires: Aug 31 20:33:05 2026 GMT
  host: www.aishub.net
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 20:33:05 2026 GMT
  host: data.aishub.net
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aishub Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AISHub, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: AISHub
provider_slug: aishub
slug: aishub-domain-security
source_filename: aishub-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aishub.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 20:33:05 2026 GMT\n  hsts: false\n- host: data.aishub.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 20:33:05 2026 GMT\n  hsts: false\ndomains:\n- domain: aishub.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aishub/refs/heads/main/security/aishub-domain-security.yml
summary_line: TLSv1.3
tags:
- Vessel Tracking
- Maritime
- AIS
- Shipping
- Geospatial
- Data Sharing
---
