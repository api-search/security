---
api_specs:
- filename: arbitron-app-account-api-openapi.yml
  format: yaml
  label: Arbitron Account API
  slug: arbitron-app-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arbitron-app/openapi/arbitron-app-account-api-openapi.yml
- filename: arbitron-app-funding-api-openapi.yml
  format: yaml
  label: Arbitron Funding API
  slug: arbitron-app-funding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arbitron-app/openapi/arbitron-app-funding-api-openapi.yml
- filename: arbitron-app-platform-api-openapi.yml
  format: yaml
  label: Arbitron Platform API
  slug: arbitron-app-platform-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arbitron-app/openapi/arbitron-app-platform-api-openapi.yml
- filename: arbitron-app-reference-data-api-openapi.yml
  format: yaml
  label: Arbitron Reference data API
  slug: arbitron-app-reference-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arbitron-app/openapi/arbitron-app-reference-data-api-openapi.yml
- filename: arbitron-app-spreads-api-openapi.yml
  format: yaml
  label: Arbitron Spreads API
  slug: arbitron-app-spreads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arbitron-app/openapi/arbitron-app-spreads-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: arbitron.app
  spf: true
hosts:
- cert_expires: Jan 10 12:20:48 2027 GMT
  host: arbitron.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Arbitron Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Arbitron, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Arbitron
provider_slug: arbitron-app
slug: arbitron-app-domain-security
source_filename: arbitron-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: arbitron.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 12:20:48 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: arbitron.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/arbitron-app/security/arbitron-app-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Cryptocurrency
- Arbitrage
- Finance
- Platform
---
