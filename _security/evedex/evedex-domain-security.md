---
api_specs:
- filename: evedex-auth-openapi.json
  format: json
  label: Auth Service
  slug: auth-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evedex/refs/heads/main/openapi/evedex-auth-openapi.json
- filename: evedex-exchange-openapi.json
  format: json
  label: Exchange Service
  slug: exchange-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evedex/refs/heads/main/openapi/evedex-exchange-openapi.json
- filename: evedex-market-data-openapi.json
  format: json
  label: Market Data Service
  slug: market-data-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evedex/refs/heads/main/openapi/evedex-market-data-openapi.json
- filename: evedex-referral-openapi.json
  format: json
  label: Referral / Affiliate Service
  slug: referral-affiliate-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evedex/refs/heads/main/openapi/evedex-referral-openapi.json
- filename: evedex-notifications-openapi.json
  format: json
  label: Notifications Service
  slug: notifications-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evedex/refs/heads/main/openapi/evedex-notifications-openapi.json
- filename: evedex-academy-openapi.json
  format: json
  label: Academy Service
  slug: academy-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evedex/refs/heads/main/openapi/evedex-academy-openapi.json
- filename: evedex-game-openapi.json
  format: json
  label: Game Service
  slug: game-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evedex/refs/heads/main/openapi/evedex-game-openapi.json
- filename: evedex-billing-openapi.json
  format: json
  label: Billing Service
  slug: billing-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evedex/refs/heads/main/openapi/evedex-billing-openapi.json
- filename: evedex-bridge-middleware-openapi.json
  format: json
  label: Bridge Middleware Service
  slug: bridge-middleware-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evedex/refs/heads/main/openapi/evedex-bridge-middleware-openapi.json
- filename: evedex-ai-strategies-openapi.json
  format: json
  label: AI Strategies Service
  slug: ai-strategies-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evedex/refs/heads/main/openapi/evedex-ai-strategies-openapi.json
- filename: evedex-backoffice-openapi.json
  format: json
  label: Backoffice Service
  slug: backoffice-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evedex/refs/heads/main/openapi/evedex-backoffice-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: evedex.com
  spf: true
hosts:
- cert_expires: Oct  1 18:29:33 2026 GMT
  host: docs.evedex.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 11 23:59:59 2027 GMT
  host: auth.evedex.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  2 23:59:59 2027 GMT
  host: swagger.evedex.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Evedex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EVEDEX, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: EVEDEX
provider_slug: evedex
slug: evedex-domain-security
source_filename: evedex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.evedex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 18:29:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: auth.evedex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 11 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: swagger.evedex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  2 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: evedex.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/evedex/refs/heads/main/security/evedex-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- cryptocurrency-exchange
- defi
- decentralized-exchange
- derivatives
- perpetual-futures
- trading
- market-data
- blockchain
- web3
- arbitrum-layer3
- fintech
---
