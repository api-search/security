---
api_specs:
- filename: placekey-openapi.yml
  format: yaml
  label: Placekey Lookup API
  slug: placekey-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/placekey/refs/heads/main/openapi/placekey-openapi.yml
- filename: placekey-openapi.yml
  format: yaml
  label: Placekey Bulk Lookup API
  slug: placekey-bulk-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/placekey/refs/heads/main/openapi/placekey-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: placekey.io
  spf: true
hosts:
- cert_expires: Sep 30 05:02:21 2026 GMT
  host: www.placekey.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 10:38:59 2026 GMT
  host: docs.placekey.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  5 23:59:59 2027 GMT
  host: api.placekey.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Placekey Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Placekey, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Placekey
provider_slug: placekey
slug: placekey-domain-security
source_filename: placekey-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.placekey.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 05:02:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.placekey.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 10:38:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.placekey.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  5 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: placekey.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/placekey/refs/heads/main/security/placekey-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Location
- Geocoding
- Address Matching
- Identifiers
- POI
---
