---
api_specs:
- filename: hathora-openapi.yml
  format: yaml
  label: Hathora Auth API
  slug: hathora-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hathora/refs/heads/main/openapi/hathora-openapi.yml
- filename: hathora-openapi.yml
  format: yaml
  label: Hathora Apps API
  slug: hathora-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hathora/refs/heads/main/openapi/hathora-openapi.yml
- filename: hathora-openapi.yml
  format: yaml
  label: Hathora Builds API
  slug: hathora-builds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hathora/refs/heads/main/openapi/hathora-openapi.yml
- filename: hathora-openapi.yml
  format: yaml
  label: Hathora Deployments API
  slug: hathora-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hathora/refs/heads/main/openapi/hathora-openapi.yml
- filename: hathora-openapi.yml
  format: yaml
  label: Hathora Processes API
  slug: hathora-processes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hathora/refs/heads/main/openapi/hathora-openapi.yml
- filename: hathora-openapi.yml
  format: yaml
  label: Hathora Rooms API
  slug: hathora-rooms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hathora/refs/heads/main/openapi/hathora-openapi.yml
- filename: hathora-openapi.yml
  format: yaml
  label: Hathora Discovery API
  slug: hathora-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hathora/refs/heads/main/openapi/hathora-openapi.yml
- filename: hathora-openapi.yml
  format: yaml
  label: Hathora Logs API
  slug: hathora-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hathora/refs/heads/main/openapi/hathora-openapi.yml
- filename: hathora-openapi.yml
  format: yaml
  label: Hathora Metrics API
  slug: hathora-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hathora/refs/heads/main/openapi/hathora-openapi.yml
- filename: hathora-openapi.yml
  format: yaml
  label: Hathora Billing API
  slug: hathora-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hathora/refs/heads/main/openapi/hathora-openapi.yml
- filename: hathora-openapi.yml
  format: yaml
  label: Hathora Tokens API
  slug: hathora-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hathora/refs/heads/main/openapi/hathora-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hathora.dev
  spf: true
hosts:
- cert_expires: Aug 16 15:25:04 2026 GMT
  host: hathora.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.hathora.dev
  https: false
kind: domain-security
layout: security
method: probed
name: Hathora Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hathora, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Hathora
provider_slug: hathora
slug: hathora-domain-security
source_filename: hathora-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hathora.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 15:25:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.hathora.dev\n  https: false\ndomains:\n- domain: hathora.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hathora/refs/heads/main/security/hathora-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Game Servers
- Multiplayer
- Compute
- Hosting
- Orchestration
---
