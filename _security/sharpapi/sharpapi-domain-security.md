---
api_specs:
- filename: sharpapi-account-api-openapi.yml
  format: yaml
  label: SharpAPI Account API
  slug: sharpapi-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sharpapi/refs/heads/main/openapi/sharpapi-account-api-openapi.yml
- filename: sharpapi-betting-splits-api-openapi.yml
  format: yaml
  label: SharpAPI Betting Splits API
  slug: sharpapi-betting-splits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sharpapi/refs/heads/main/openapi/sharpapi-betting-splits-api-openapi.yml
- filename: sharpapi-deep-links-api-openapi.yml
  format: yaml
  label: SharpAPI Deep Links API
  slug: sharpapi-deep-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sharpapi/refs/heads/main/openapi/sharpapi-deep-links-api-openapi.yml
- filename: sharpapi-events-api-openapi.yml
  format: yaml
  label: SharpAPI Events API
  slug: sharpapi-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sharpapi/refs/heads/main/openapi/sharpapi-events-api-openapi.yml
- filename: sharpapi-futures-api-openapi.yml
  format: yaml
  label: SharpAPI Futures API
  slug: sharpapi-futures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sharpapi/refs/heads/main/openapi/sharpapi-futures-api-openapi.yml
- filename: sharpapi-game-state-api-openapi.yml
  format: yaml
  label: SharpAPI Game State API
  slug: sharpapi-game-state-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sharpapi/refs/heads/main/openapi/sharpapi-game-state-api-openapi.yml
- filename: sharpapi-health-api-openapi.yml
  format: yaml
  label: SharpAPI Health API
  slug: sharpapi-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sharpapi/refs/heads/main/openapi/sharpapi-health-api-openapi.yml
- filename: sharpapi-odds-api-openapi.yml
  format: yaml
  label: SharpAPI Odds API
  slug: sharpapi-odds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sharpapi/refs/heads/main/openapi/sharpapi-odds-api-openapi.yml
- filename: sharpapi-opportunities-api-openapi.yml
  format: yaml
  label: SharpAPI Opportunities API
  slug: sharpapi-opportunities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sharpapi/refs/heads/main/openapi/sharpapi-opportunities-api-openapi.yml
- filename: sharpapi-reference-data-api-openapi.yml
  format: yaml
  label: SharpAPI Reference Data API
  slug: sharpapi-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sharpapi/refs/heads/main/openapi/sharpapi-reference-data-api-openapi.yml
- filename: sharpapi-streaming-api-openapi.yml
  format: yaml
  label: SharpAPI Streaming API
  slug: sharpapi-streaming-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sharpapi/refs/heads/main/openapi/sharpapi-streaming-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sharpapi.io
  spf: true
hosts:
- cert_expires: Dec 25 01:58:58 2026 GMT
  host: sharpapi.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Sharpapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SharpAPI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SharpAPI
provider_slug: sharpapi
slug: sharpapi-domain-security
source_filename: sharpapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sharpapi.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 01:58:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sharpapi.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sharpapi/refs/heads/main/security/sharpapi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Sports Betting
- Real-Time Data
- Gambling
---
