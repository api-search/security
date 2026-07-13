---
api_specs:
- filename: sportradar-sports-data-openapi.yml
  format: yaml
  label: Sportradar Sports Data API
  slug: sports-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sportradar/refs/heads/main/openapi/sportradar-sports-data-openapi.yml
- filename: sportradar-push-feeds-openapi.yml
  format: yaml
  label: Sportradar Push Feeds API
  slug: push-feeds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sportradar/refs/heads/main/openapi/sportradar-push-feeds-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sportradar.com
  spf: true
hosts:
- cert_expires: Sep 22 01:36:45 2026 GMT
  host: developer.sportradar.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 01:43:31 2026 GMT
  host: sportradar.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  6 23:59:59 2027 GMT
  host: api.sportradar.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sportradar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sportradar, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Sportradar
provider_slug: sportradar
slug: sportradar-domain-security
source_filename: sportradar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.sportradar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 01:36:45 2026 GMT\n  hsts: null\n- host: sportradar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 01:43:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.sportradar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  6 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: sportradar.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sportradar/refs/heads/main/security/sportradar-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Data
- Esports
- Fantasy Sports
- HTTP Chunked
- Media
- Push
- Real-Time
- Sports
- Sports Data
- Statistics
- Streaming
---
