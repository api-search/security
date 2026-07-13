---
api_specs:
- filename: geocodio-openapi.yml
  format: yaml
  label: Geocodio Forward Geocoding
  slug: forward-geocoding
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/geocodio/refs/heads/main/openapi/geocodio-openapi.yml
- filename: geocodio-openapi.yml
  format: yaml
  label: Geocodio Reverse Geocoding
  slug: reverse-geocoding
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/geocodio/refs/heads/main/openapi/geocodio-openapi.yml
- filename: geocodio-openapi.yml
  format: yaml
  label: Geocodio Batch Geocoding
  slug: batch-geocoding
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/geocodio/refs/heads/main/openapi/geocodio-openapi.yml
- filename: geocodio-openapi.yml
  format: yaml
  label: Geocodio Data Appends
  slug: data-appends
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/geocodio/refs/heads/main/openapi/geocodio-openapi.yml
- filename: geocodio-openapi.yml
  format: yaml
  label: Geocodio Lists
  slug: lists
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/geocodio/refs/heads/main/openapi/geocodio-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: geocod.io
  spf: true
hosts:
- cert_expires: Oct  3 13:30:28 2026 GMT
  host: www.geocod.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 13:06:44 2026 GMT
  host: api.geocod.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Geocodio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Geocodio, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Geocodio
provider_slug: geocodio
slug: geocodio-domain-security
source_filename: geocodio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.geocod.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 13:30:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.geocod.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 13:06:44 2026 GMT\n  hsts: false\ndomains:\n- domain: geocod.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/geocodio/refs/heads/main/security/geocodio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Geocoding
- Reverse Geocoding
- Addresses
- Data Append
- Census
---
