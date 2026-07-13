---
api_specs:
- filename: mapbox-openapi.yml
  format: yaml
  label: Mapbox Tiling Service
  slug: mapbox-tiling-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mapbox/refs/heads/main/openapi/mapbox-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mapbox.com
  spf: true
hosts:
- cert_expires: Jan  9 23:00:19 2027 GMT
  host: www.mapbox.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct  4 23:59:59 2026 GMT
  host: docs.mapbox.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 23:59:59 2026 GMT
  host: api.mapbox.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mapbox Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mapbox, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Mapbox
provider_slug: mapbox
slug: mapbox-domain-security
source_filename: mapbox-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mapbox.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  9 23:00:19 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.mapbox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.mapbox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: mapbox.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mapbox/refs/heads/main/security/mapbox-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Mapping
- Maps
- Geospatial
- Location
---
