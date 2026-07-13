---
api_specs:
- filename: imdb-api-openapi.yml
  format: yaml
  label: IMDb-API
  slug: imdb-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/imdb-api/refs/heads/main/openapi/imdb-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tv-api.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: imdb-api.com
  spf: true
hosts:
- cert_expires: Sep 19 09:15:12 2026 GMT
  host: tv-api.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- host: imdb-api.com
  https: false
kind: domain-security
layout: security
method: probed
name: Imdb Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IMDb-API, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: IMDb-API
provider_slug: imdb-api
slug: imdb-api-domain-security
source_filename: imdb-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tv-api.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 09:15:12 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: imdb-api.com\n  https: false\ndomains:\n- domain: tv-api.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: imdb-api.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/imdb-api/refs/heads/main/security/imdb-api-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Video
- Movies
- TV
- Entertainment
- Metadata
- Ratings
- Public APIs
---
