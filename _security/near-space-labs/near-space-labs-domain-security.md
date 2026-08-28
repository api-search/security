---
api_specs:
- filename: near-space-labs-tile-service.json
  format: json
  label: Near Space Labs Tile Service
  slug: near-space-labs-tile-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/near-space-labs/refs/heads/main/openapi/near-space-labs-tile-service.json
- filename: near-space-labs-oauth-service.json
  format: json
  label: Near Space Labs OAuth Service
  slug: near-space-labs-oauth-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/near-space-labs/refs/heads/main/openapi/near-space-labs-oauth-service.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nearspacelabs.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: nearspacelabs.net
  spf: false
hosts:
- cert_expires: Oct 27 01:49:19 2026 GMT
  host: www.nearspacelabs.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 21 15:19:36 2026 GMT
  host: docs.nearspacelabs.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 30 14:27:02 2026 GMT
  host: api.nearspacelabs.net
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Near Space Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Near Space Labs, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Near Space Labs
provider_slug: near-space-labs
slug: near-space-labs-domain-security
source_filename: near-space-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nearspacelabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 01:49:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.nearspacelabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 15:19:36 2026 GMT\n  hsts: false\n- host: api.nearspacelabs.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 14:27:02 2026 GMT\n  hsts: null\ndomains:\n- domain: nearspacelabs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: nearspacelabs.net\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/near-space-labs/refs/heads/main/security/near-space-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Earth Observation
- Aerial Imagery
- Geospatial
- Satellite and Remote Sensing
- Mapping
- Tiles
- Insurance
- Government
- Utilities
- Location
- Imagery
---
