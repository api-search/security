---
api_specs:
- filename: gracenote-celebrities-api-openapi.yml
  format: yaml
  label: Gracenote Celebrities API
  slug: gracenote-celebrities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gracenote/refs/heads/main/openapi/gracenote-celebrities-api-openapi.yml
- filename: gracenote-lineups-api-openapi.yml
  format: yaml
  label: Gracenote Lineups API
  slug: gracenote-lineups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gracenote/refs/heads/main/openapi/gracenote-lineups-api-openapi.yml
- filename: gracenote-movies-api-openapi.yml
  format: yaml
  label: Gracenote Movies API
  slug: gracenote-movies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gracenote/refs/heads/main/openapi/gracenote-movies-api-openapi.yml
- filename: gracenote-programs-api-openapi.yml
  format: yaml
  label: Gracenote Programs API
  slug: gracenote-programs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gracenote/refs/heads/main/openapi/gracenote-programs-api-openapi.yml
- filename: gracenote-series-api-openapi.yml
  format: yaml
  label: Gracenote Series API
  slug: gracenote-series-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gracenote/refs/heads/main/openapi/gracenote-series-api-openapi.yml
- filename: gracenote-sports-api-openapi.yml
  format: yaml
  label: Gracenote Sports API
  slug: gracenote-sports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gracenote/refs/heads/main/openapi/gracenote-sports-api-openapi.yml
- filename: gracenote-stations-api-openapi.yml
  format: yaml
  label: Gracenote Stations API
  slug: gracenote-stations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gracenote/refs/heads/main/openapi/gracenote-stations-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gracenote.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: tmsapi.com
  spf: false
hosts:
- cert_expires: Sep 25 00:34:27 2026 GMT
  host: www.gracenote.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 31 13:11:20 2026 GMT
  host: developer.tmsapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 31 13:11:20 2026 GMT
  host: data.tmsapi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gracenote Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gracenote, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Gracenote
provider_slug: gracenote
slug: gracenote-domain-security
source_filename: gracenote-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gracenote.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 00:34:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.tmsapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 13:11:20 2026 GMT\n  hsts: false\n- host: data.tmsapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 13:11:20 2026 GMT\n  hsts: null\ndomains:\n- domain: gracenote.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: tmsapi.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gracenote/refs/heads/main/security/gracenote-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Automotive
- Content Metadata
- Entertainment
- Music
- Nielsen
- Sports
- Streaming
- Television
- Video
---
