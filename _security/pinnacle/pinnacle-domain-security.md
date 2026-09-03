---
api_specs:
- filename: pinnacle-asyncapi.yml
  format: yaml
  label: Pinnacle Lines API
  slug: pinnacle-lines-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinnacle/refs/heads/main/openapi/pinnacle-asyncapi.yml
- filename: pinnacle-cancellationreasons-api-openapi.yml
  format: yaml
  label: ' Pinnacle Sports Betting Cancellationreasons API'
  slug: pinnacle-cancellationreasons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinnacle/refs/heads/main/openapi/pinnacle-cancellationreasons-api-openapi.yml
- filename: pinnacle-currencies-api-openapi.yml
  format: yaml
  label: ' Pinnacle Sports Betting Currencies API'
  slug: pinnacle-currencies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinnacle/refs/heads/main/openapi/pinnacle-currencies-api-openapi.yml
- filename: pinnacle-fixtures-api-openapi.yml
  format: yaml
  label: ' Pinnacle Sports Betting Fixtures API'
  slug: pinnacle-fixtures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinnacle/refs/heads/main/openapi/pinnacle-fixtures-api-openapi.yml
- filename: pinnacle-inrunning-api-openapi.yml
  format: yaml
  label: ' Pinnacle Sports Betting Inrunning API'
  slug: pinnacle-inrunning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinnacle/refs/heads/main/openapi/pinnacle-inrunning-api-openapi.yml
- filename: pinnacle-leagues-api-openapi.yml
  format: yaml
  label: ' Pinnacle Sports Betting Leagues API'
  slug: pinnacle-leagues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinnacle/refs/heads/main/openapi/pinnacle-leagues-api-openapi.yml
- filename: pinnacle-line-api-openapi.yml
  format: yaml
  label: ' Pinnacle Sports Betting Line API'
  slug: pinnacle-line-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinnacle/refs/heads/main/openapi/pinnacle-line-api-openapi.yml
- filename: pinnacle-odds-api-openapi.yml
  format: yaml
  label: ' Pinnacle Sports Betting Odds API'
  slug: pinnacle-odds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinnacle/refs/heads/main/openapi/pinnacle-odds-api-openapi.yml
- filename: pinnacle-periods-api-openapi.yml
  format: yaml
  label: ' Pinnacle Sports Betting Periods API'
  slug: pinnacle-periods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinnacle/refs/heads/main/openapi/pinnacle-periods-api-openapi.yml
- filename: pinnacle-sports-api-openapi.yml
  format: yaml
  label: ' Pinnacle Sports Betting Sports API'
  slug: pinnacle-sports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinnacle/refs/heads/main/openapi/pinnacle-sports-api-openapi.yml
- filename: pinnacle-teaser-api-openapi.yml
  format: yaml
  label: ' Pinnacle Sports Betting Teaser API'
  slug: pinnacle-teaser-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinnacle/refs/heads/main/openapi/pinnacle-teaser-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pinnacle.com
  spf: true
hosts:
- cert_expires: Sep 22 17:18:28 2026 GMT
  host: www.pinnacle.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 17:18:28 2026 GMT
  host: api.pinnacle.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pinnacle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pinnacle Sports Betting, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Pinnacle Sports Betting
provider_slug: pinnacle
slug: pinnacle-domain-security
source_filename: pinnacle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pinnacle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 17:18:28 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: api.pinnacle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 17:18:28 2026 GMT\n  hsts: null\ndomains:\n- domain: pinnacle.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pinnacle/refs/heads/main/security/pinnacle-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Gambling
- Sports Betting
---
