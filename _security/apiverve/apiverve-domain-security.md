---
api_specs:
- filename: apiverve-openapi.yaml
  format: yaml
  label: APIVerve REST API
  slug: apiverve-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiverve/refs/heads/main/openapi/apiverve-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: apiverve.com
  spf: true
hosts:
- cert_expires: Dec  6 21:44:57 2026 GMT
  host: docs.apiverve.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 15 07:04:39 2026 GMT
  host: api.apiverve.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.2
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Apiverve Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for APIVerve, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: APIVerve
provider_slug: apiverve
slug: apiverve-domain-security
source_filename: apiverve-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.apiverve.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  6 21:44:57 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: api.apiverve.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 15 07:04:39 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: apiverve.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apiverve/refs/heads/main/security/apiverve-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- API Marketplace
- REST
- JSON
- GraphQL
- OpenAPI
- Postman
- MCP
- llms-txt
- agent-native
- APIKeys
- IP Geolocation
- DNS
- WHOIS
- SSL
- Email Validation
- Phone Validation
- Exchange Rates
- metals prices
- Weather
- Geocoding
- Text Processing
- Developer Tools
---
