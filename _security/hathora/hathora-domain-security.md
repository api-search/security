---
api_specs:
- filename: hathora-appsv2-api-openapi.yml
  format: yaml
  label: Hathora AppsV2 API
  slug: hathora-appsv2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hathora/refs/heads/main/openapi/hathora-appsv2-api-openapi.yml
- filename: hathora-authv1-api-openapi.yml
  format: yaml
  label: Hathora AuthV1 API
  slug: hathora-authv1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hathora/refs/heads/main/openapi/hathora-authv1-api-openapi.yml
- filename: hathora-billingv1-api-openapi.yml
  format: yaml
  label: Hathora BillingV1 API
  slug: hathora-billingv1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hathora/refs/heads/main/openapi/hathora-billingv1-api-openapi.yml
- filename: hathora-buildsv3-api-openapi.yml
  format: yaml
  label: Hathora BuildsV3 API
  slug: hathora-buildsv3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hathora/refs/heads/main/openapi/hathora-buildsv3-api-openapi.yml
- filename: hathora-deploymentsv3-api-openapi.yml
  format: yaml
  label: Hathora DeploymentsV3 API
  slug: hathora-deploymentsv3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hathora/refs/heads/main/openapi/hathora-deploymentsv3-api-openapi.yml
- filename: hathora-discoveryv2-api-openapi.yml
  format: yaml
  label: Hathora DiscoveryV2 API
  slug: hathora-discoveryv2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hathora/refs/heads/main/openapi/hathora-discoveryv2-api-openapi.yml
- filename: hathora-logsv1-api-openapi.yml
  format: yaml
  label: Hathora LogsV1 API
  slug: hathora-logsv1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hathora/refs/heads/main/openapi/hathora-logsv1-api-openapi.yml
- filename: hathora-metricsv1-api-openapi.yml
  format: yaml
  label: Hathora MetricsV1 API
  slug: hathora-metricsv1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hathora/refs/heads/main/openapi/hathora-metricsv1-api-openapi.yml
- filename: hathora-processesv3-api-openapi.yml
  format: yaml
  label: Hathora ProcessesV3 API
  slug: hathora-processesv3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hathora/refs/heads/main/openapi/hathora-processesv3-api-openapi.yml
- filename: hathora-roomsv2-api-openapi.yml
  format: yaml
  label: Hathora RoomsV2 API
  slug: hathora-roomsv2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hathora/refs/heads/main/openapi/hathora-roomsv2-api-openapi.yml
- filename: hathora-tokensv1-api-openapi.yml
  format: yaml
  label: Hathora TokensV1 API
  slug: hathora-tokensv1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hathora/refs/heads/main/openapi/hathora-tokensv1-api-openapi.yml
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
