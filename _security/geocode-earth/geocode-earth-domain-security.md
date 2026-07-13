---
api_specs:
- filename: geocode-earth-openapi.yml
  format: yaml
  label: Geocode Earth Search API
  slug: search
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/geocode-earth/refs/heads/main/openapi/geocode-earth-openapi.yml
- filename: geocode-earth-openapi.yml
  format: yaml
  label: Geocode Earth Autocomplete API
  slug: autocomplete
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/geocode-earth/refs/heads/main/openapi/geocode-earth-openapi.yml
- filename: geocode-earth-openapi.yml
  format: yaml
  label: Geocode Earth Reverse API
  slug: reverse
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/geocode-earth/refs/heads/main/openapi/geocode-earth-openapi.yml
- filename: geocode-earth-openapi.yml
  format: yaml
  label: Geocode Earth Structured Search API
  slug: structured-search
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/geocode-earth/refs/heads/main/openapi/geocode-earth-openapi.yml
- filename: geocode-earth-openapi.yml
  format: yaml
  label: Geocode Earth Place API
  slug: place
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/geocode-earth/refs/heads/main/openapi/geocode-earth-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: geocode.earth
  spf: true
hosts:
- cert_expires: Sep 14 19:34:02 2026 GMT
  host: geocode.earth
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  7 23:59:59 2026 GMT
  host: api.geocode.earth
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Geocode Earth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Geocode Earth, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Geocode Earth
provider_slug: geocode-earth
slug: geocode-earth-domain-security
source_filename: geocode-earth-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: geocode.earth\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 19:34:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.geocode.earth\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: geocode.earth\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/geocode-earth/refs/heads/main/security/geocode-earth-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Geocoding
- Address Autocomplete
- Reverse Geocoding
- Mapping
- Pelias
- Open Data
---
