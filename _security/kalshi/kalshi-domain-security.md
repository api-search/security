---
api_specs:
- filename: asyncapi.yaml
  format: yaml
  label: Kalshi WebSocket Streaming API
  slug: websocket
  spec_type: AsyncAPI
  url: https://docs.kalshi.com/asyncapi.yaml
- filename: asyncapi.yaml
  format: yaml
  label: Kalshi AsyncAPI Specification
  slug: asyncapi
  spec_type: AsyncAPI
  url: https://docs.kalshi.com/asyncapi.yaml
- filename: kalshi-account-api-openapi.yml
  format: yaml
  label: Kalshi account API
  slug: kalshi-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kalshi/refs/heads/main/openapi/kalshi-account-api-openapi.yml
- filename: kalshi-api-keys-api-openapi.yml
  format: yaml
  label: Kalshi api-keys API
  slug: kalshi-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kalshi/refs/heads/main/openapi/kalshi-api-keys-api-openapi.yml
- filename: kalshi-communications-api-openapi.yml
  format: yaml
  label: Kalshi communications API
  slug: kalshi-communications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kalshi/refs/heads/main/openapi/kalshi-communications-api-openapi.yml
- filename: kalshi-events-api-openapi.yml
  format: yaml
  label: Kalshi events API
  slug: kalshi-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kalshi/refs/heads/main/openapi/kalshi-events-api-openapi.yml
- filename: kalshi-exchange-api-openapi.yml
  format: yaml
  label: Kalshi exchange API
  slug: kalshi-exchange-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kalshi/refs/heads/main/openapi/kalshi-exchange-api-openapi.yml
- filename: kalshi-fcm-api-openapi.yml
  format: yaml
  label: Kalshi fcm API
  slug: kalshi-fcm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kalshi/refs/heads/main/openapi/kalshi-fcm-api-openapi.yml
- filename: kalshi-historical-api-openapi.yml
  format: yaml
  label: Kalshi historical API
  slug: kalshi-historical-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kalshi/refs/heads/main/openapi/kalshi-historical-api-openapi.yml
- filename: kalshi-incentive-programs-api-openapi.yml
  format: yaml
  label: Kalshi incentive-programs API
  slug: kalshi-incentive-programs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kalshi/refs/heads/main/openapi/kalshi-incentive-programs-api-openapi.yml
- filename: kalshi-live-data-api-openapi.yml
  format: yaml
  label: Kalshi live-data API
  slug: kalshi-live-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kalshi/refs/heads/main/openapi/kalshi-live-data-api-openapi.yml
- filename: kalshi-market-api-openapi.yml
  format: yaml
  label: Kalshi market API
  slug: kalshi-market-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kalshi/refs/heads/main/openapi/kalshi-market-api-openapi.yml
- filename: kalshi-milestone-api-openapi.yml
  format: yaml
  label: Kalshi milestone API
  slug: kalshi-milestone-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kalshi/refs/heads/main/openapi/kalshi-milestone-api-openapi.yml
- filename: kalshi-multivariate-api-openapi.yml
  format: yaml
  label: Kalshi multivariate API
  slug: kalshi-multivariate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kalshi/refs/heads/main/openapi/kalshi-multivariate-api-openapi.yml
- filename: kalshi-order-groups-api-openapi.yml
  format: yaml
  label: Kalshi order-groups API
  slug: kalshi-order-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kalshi/refs/heads/main/openapi/kalshi-order-groups-api-openapi.yml
- filename: kalshi-orders-api-openapi.yml
  format: yaml
  label: Kalshi orders API
  slug: kalshi-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kalshi/refs/heads/main/openapi/kalshi-orders-api-openapi.yml
- filename: kalshi-portfolio-api-openapi.yml
  format: yaml
  label: Kalshi portfolio API
  slug: kalshi-portfolio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kalshi/refs/heads/main/openapi/kalshi-portfolio-api-openapi.yml
- filename: kalshi-search-api-openapi.yml
  format: yaml
  label: Kalshi search API
  slug: kalshi-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kalshi/refs/heads/main/openapi/kalshi-search-api-openapi.yml
- filename: kalshi-structured-targets-api-openapi.yml
  format: yaml
  label: Kalshi structured-targets API
  slug: kalshi-structured-targets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kalshi/refs/heads/main/openapi/kalshi-structured-targets-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "awstrust.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: kalshi.com
  spf: true
hosts:
- cert_expires: Aug 24 06:05:39 2026 GMT
  host: kalshi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 10 00:20:33 2026 GMT
  host: docs.kalshi.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 23:59:59 2026 GMT
  host: api.elections.kalshi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kalshi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kalshi, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Kalshi
provider_slug: kalshi
slug: kalshi-domain-security
source_filename: kalshi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kalshi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 06:05:39 2026 GMT\n  hsts: null\n- host: docs.kalshi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 10 00:20:33 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.elections.kalshi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: kalshi.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kalshi/refs/heads/main/security/kalshi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Prediction Markets
- Event Contracts
- Exchange
- CFTC
- Trading
- Markets
---
