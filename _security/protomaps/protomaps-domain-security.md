---
api_specs:
- filename: api
  format: yaml
  label: Protomaps Hosted Tile API
  slug: protomaps-hosted-tile-api
  spec_type: OpenAPI
  url: https://protomaps.com/api
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: protomaps.com
  spf: true
hosts:
- cert_expires: Oct  2 05:47:55 2026 GMT
  host: protomaps.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  8 08:01:10 2026 GMT
  host: api.protomaps.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 00:51:00 2026 GMT
  host: docs.protomaps.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Protomaps Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Protomaps, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Protomaps
provider_slug: protomaps
slug: protomaps-domain-security
source_filename: protomaps-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: protomaps.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 05:47:55 2026 GMT\n  hsts: false\n- host: api.protomaps.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 08:01:10 2026 GMT\n  hsts: null\n- host: docs.protomaps.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 00:51:00 2026 GMT\n  hsts: false\ndomains:\n- domain: protomaps.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/protomaps/refs/heads/main/security/protomaps-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Maps
- Tiles
- Geospatial
- PMTiles
- Vector Tiles
- Open Source
- Self-Hosted
- OpenStreetMap
---
