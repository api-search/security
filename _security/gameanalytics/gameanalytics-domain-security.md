---
api_specs:
- filename: gameanalytics-openapi.yml
  format: yaml
  label: GameAnalytics Collection API
  slug: gameanalytics-collection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gameanalytics/refs/heads/main/openapi/gameanalytics-openapi.yml
- filename: gameanalytics-openapi.yml
  format: yaml
  label: GameAnalytics Metrics API
  slug: gameanalytics-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gameanalytics/refs/heads/main/openapi/gameanalytics-openapi.yml
- filename: gameanalytics-openapi.yml
  format: yaml
  label: GameAnalytics Organization API
  slug: gameanalytics-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gameanalytics/refs/heads/main/openapi/gameanalytics-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gameanalytics.com
  spf: true
hosts:
- cert_expires: Aug 16 17:18:30 2026 GMT
  host: gameanalytics.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  5 23:59:59 2026 GMT
  host: docs.gameanalytics.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 20 23:59:59 2027 GMT
  host: api.gameanalytics.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gameanalytics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GameAnalytics, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: GameAnalytics
provider_slug: gameanalytics
slug: gameanalytics-domain-security
source_filename: gameanalytics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gameanalytics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 17:18:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.gameanalytics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 23:59:59 2026 GMT\n  hsts: false\n- host: api.gameanalytics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 20 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: gameanalytics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gameanalytics/refs/heads/main/security/gameanalytics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- Games
- Gaming
- Player Behavior
- Retention
- Monetization
- Ad Analytics
- Telemetry
---
