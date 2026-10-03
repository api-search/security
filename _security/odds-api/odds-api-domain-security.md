---
api_specs:
- filename: odds-api-account-api-openapi.yml
  format: yaml
  label: Odds API Account API
  slug: odds-api-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/odds-api/refs/heads/main/openapi/odds-api-account-api-openapi.yml
- filename: odds-api-betting-opportunities-api-openapi.yml
  format: yaml
  label: Odds API Betting opportunities API
  slug: odds-api-betting-opportunities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/odds-api/refs/heads/main/openapi/odds-api-betting-opportunities-api-openapi.yml
- filename: odds-api-catalog-api-openapi.yml
  format: yaml
  label: Odds API Catalog API
  slug: odds-api-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/odds-api/refs/heads/main/openapi/odds-api-catalog-api-openapi.yml
- filename: odds-api-prediction-markets-api-openapi.yml
  format: yaml
  label: Odds API Prediction markets API
  slug: odds-api-prediction-markets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/odds-api/refs/heads/main/openapi/odds-api-prediction-markets-api-openapi.yml
- filename: odds-api-racing-events-api-openapi.yml
  format: yaml
  label: Odds API Racing events API
  slug: odds-api-racing-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/odds-api/refs/heads/main/openapi/odds-api-racing-events-api-openapi.yml
- filename: odds-api-racing-odds-api-openapi.yml
  format: yaml
  label: Odds API Racing odds API
  slug: odds-api-racing-odds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/odds-api/refs/heads/main/openapi/odds-api-racing-odds-api-openapi.yml
- filename: odds-api-results-api-openapi.yml
  format: yaml
  label: Odds API Results API
  slug: odds-api-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/odds-api/refs/heads/main/openapi/odds-api-results-api-openapi.yml
- filename: odds-api-sports-events-api-openapi.yml
  format: yaml
  label: Odds API Sports events API
  slug: odds-api-sports-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/odds-api/refs/heads/main/openapi/odds-api-sports-events-api-openapi.yml
- filename: odds-api-sports-exchange-api-openapi.yml
  format: yaml
  label: Odds API Sports exchange API
  slug: odds-api-sports-exchange-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/odds-api/refs/heads/main/openapi/odds-api-sports-exchange-api-openapi.yml
- filename: odds-api-sports-odds-api-openapi.yml
  format: yaml
  label: Odds API Sports odds API
  slug: odds-api-sports-odds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/odds-api/refs/heads/main/openapi/odds-api-sports-odds-api-openapi.yml
- filename: odds-api-start-here-api-openapi.yml
  format: yaml
  label: Odds API Start here API
  slug: odds-api-start-here-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/odds-api/refs/heads/main/openapi/odds-api-start-here-api-openapi.yml
- filename: odds-api-status-api-openapi.yml
  format: yaml
  label: Odds API Status API
  slug: odds-api-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/odds-api/refs/heads/main/openapi/odds-api-status-api-openapi.yml
- filename: odds-api-widgets-api-openapi.yml
  format: yaml
  label: Odds API Widgets API
  slug: odds-api-widgets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/odds-api/refs/heads/main/openapi/odds-api-widgets-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: odds-api.net
  spf: true
hosts:
- cert_expires: Nov 20 00:04:03 2026 GMT
  host: odds-api.net
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 26 22:21:59 2026 GMT
  host: api.odds-api.net
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Odds Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Odds API, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Odds API
provider_slug: odds-api
slug: odds-api-domain-security
source_filename: odds-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: odds-api.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 00:04:03 2026 GMT\n  hsts: false\n- host: api.odds-api.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 22:21:59 2026 GMT\n  hsts: null\ndomains:\n- domain: odds-api.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/odds-api/refs/heads/main/security/odds-api-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Sports
- Sports Betting
- betting-odds
- bookmaker-odds
- live-odds
- Sportsbook
- Racing
- REST
- Server-Sent Events
- WebSocket
- OpenAPI
- MCP
- Agent-Native
- llms-txt
- SDK
- Postman
---
