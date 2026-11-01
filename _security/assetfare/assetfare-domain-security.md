---
api_specs:
- filename: assetfare-capabilities-api-openapi.yml
  format: yaml
  label: AssetFare Capabilities API
  slug: assetfare-capabilities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/assetfare/openapi/assetfare-capabilities-api-openapi.yml
- filename: assetfare-prepare-api-openapi.yml
  format: yaml
  label: AssetFare Prepare API
  slug: assetfare-prepare-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/assetfare/openapi/assetfare-prepare-api-openapi.yml
- filename: assetfare-quote-api-openapi.yml
  format: yaml
  label: AssetFare Quote API
  slug: assetfare-quote-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/assetfare/openapi/assetfare-quote-api-openapi.yml
- filename: assetfare-session-api-openapi.yml
  format: yaml
  label: AssetFare Session API
  slug: assetfare-session-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/assetfare/openapi/assetfare-session-api-openapi.yml
- filename: assetfare-status-api-openapi.yml
  format: yaml
  label: AssetFare Status API
  slug: assetfare-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/assetfare/openapi/assetfare-status-api-openapi.yml
- filename: assetfare-app-store-api-openapi.yml
  format: yaml
  label: AssetFare App Store API
  slug: assetfare-app-store-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/assetfare/openapi/assetfare-app-store-api-openapi.yml
- filename: assetfare-auth-api-openapi.yml
  format: yaml
  label: AssetFare Auth API
  slug: assetfare-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/assetfare/openapi/assetfare-auth-api-openapi.yml
- filename: assetfare-events-api-openapi.yml
  format: yaml
  label: AssetFare Events API
  slug: assetfare-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/assetfare/openapi/assetfare-events-api-openapi.yml
- filename: assetfare-google-play-api-openapi.yml
  format: yaml
  label: AssetFare Google Play API
  slug: assetfare-google-play-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/assetfare/openapi/assetfare-google-play-api-openapi.yml
- filename: assetfare-jobs-api-openapi.yml
  format: yaml
  label: AssetFare Jobs API
  slug: assetfare-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/assetfare/openapi/assetfare-jobs-api-openapi.yml
- filename: assetfare-route-selection-api-openapi.yml
  format: yaml
  label: AssetFare Route Selection API
  slug: assetfare-route-selection-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/assetfare/openapi/assetfare-route-selection-api-openapi.yml
- filename: assetfare-well-known-api-openapi.yml
  format: yaml
  label: AssetFare .well Known API
  slug: assetfare-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/assetfare/openapi/assetfare-well-known-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: assetfare.dev
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: appstorespy.com
  spf: true
hosts:
- cert_expires: Jan  3 12:52:05 2027 GMT
  host: assetfare.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 13 01:46:12 2026 GMT
  host: api.assetfare.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 19 16:02:24 2027 GMT
  host: api.appstorespy.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Assetfare Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AssetFare, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: AssetFare
provider_slug: assetfare
slug: assetfare-domain-security
source_filename: assetfare-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: assetfare.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 12:52:05 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.assetfare.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 01:46:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.appstorespy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 16:02:24 2027 GMT\n  hsts: false\ndomains:\n- domain: assetfare.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: appstorespy.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/assetfare/security/assetfare-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI Agents
- Asset Transfer
- Bridge
- Cross-Chain
- Non-Custodial
- Cryptocurrency
- Solana
- Base
- Arbitrum
- Robinhood Chain
- Optimism
- Ethereum
- OpenAPI
- MCP
- Agent Skills
---
