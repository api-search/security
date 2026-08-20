---
api_specs:
- filename: boltic-tables-api-openapi.yml
  format: yaml
  label: Boltic Tables API
  slug: tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boltic/refs/heads/main/openapi/boltic-tables-api-openapi.yml
- filename: boltic-pipes-api-openapi.yml
  format: yaml
  label: Boltic Pipes API
  slug: pipes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boltic/refs/heads/main/openapi/boltic-pipes-api-openapi.yml
- filename: boltic-certificates-api-openapi.yml
  format: yaml
  label: Boltic Certificates API
  slug: boltic-certificates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boltic/refs/heads/main/openapi/boltic-certificates-api-openapi.yml
- filename: boltic-consumers-api-openapi.yml
  format: yaml
  label: Boltic Consumers API
  slug: boltic-consumers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boltic/refs/heads/main/openapi/boltic-consumers-api-openapi.yml
- filename: boltic-destinations-api-openapi.yml
  format: yaml
  label: Boltic Destinations API
  slug: boltic-destinations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boltic/refs/heads/main/openapi/boltic-destinations-api-openapi.yml
- filename: boltic-events-api-openapi.yml
  format: yaml
  label: Boltic Events API
  slug: boltic-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boltic/refs/heads/main/openapi/boltic-events-api-openapi.yml
- filename: boltic-executions-api-openapi.yml
  format: yaml
  label: Boltic Executions API
  slug: boltic-executions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boltic/refs/heads/main/openapi/boltic-executions-api-openapi.yml
- filename: boltic-plugins-api-openapi.yml
  format: yaml
  label: Boltic Plugins API
  slug: boltic-plugins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boltic/refs/heads/main/openapi/boltic-plugins-api-openapi.yml
- filename: boltic-queries-api-openapi.yml
  format: yaml
  label: Boltic Queries API
  slug: boltic-queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boltic/refs/heads/main/openapi/boltic-queries-api-openapi.yml
- filename: boltic-routes-api-openapi.yml
  format: yaml
  label: Boltic Routes API
  slug: boltic-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boltic/refs/heads/main/openapi/boltic-routes-api-openapi.yml
- filename: boltic-rows-api-openapi.yml
  format: yaml
  label: Boltic Rows API
  slug: boltic-rows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boltic/refs/heads/main/openapi/boltic-rows-api-openapi.yml
- filename: boltic-services-api-openapi.yml
  format: yaml
  label: Boltic Services API
  slug: boltic-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boltic/refs/heads/main/openapi/boltic-services-api-openapi.yml
- filename: boltic-sources-api-openapi.yml
  format: yaml
  label: Boltic Sources API
  slug: boltic-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boltic/refs/heads/main/openapi/boltic-sources-api-openapi.yml
- filename: boltic-stream-sources-api-openapi.yml
  format: yaml
  label: Boltic Stream Sources API
  slug: boltic-stream-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boltic/refs/heads/main/openapi/boltic-stream-sources-api-openapi.yml
- filename: boltic-sync-runs-api-openapi.yml
  format: yaml
  label: Boltic Sync Runs API
  slug: boltic-sync-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boltic/refs/heads/main/openapi/boltic-sync-runs-api-openapi.yml
- filename: boltic-triggers-api-openapi.yml
  format: yaml
  label: Boltic Triggers API
  slug: boltic-triggers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boltic/refs/heads/main/openapi/boltic-triggers-api-openapi.yml
- filename: boltic-workflows-api-openapi.yml
  format: yaml
  label: Boltic Workflows API
  slug: boltic-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boltic/refs/heads/main/openapi/boltic-workflows-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: boltic.io
  spf: true
hosts:
- cert_expires: Sep 14 12:02:43 2026 GMT
  host: www.boltic.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 09:01:49 2026 GMT
  host: docs.boltic.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 16 18:12:21 2026 GMT
  host: gateway.boltic.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Boltic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Boltic, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Boltic
provider_slug: boltic
slug: boltic-domain-security
source_filename: boltic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.boltic.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 12:02:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.boltic.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 09:01:49 2026 GMT\n  hsts: false\n- host: gateway.boltic.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 18:12:21 2026 GMT\n  hsts: null\ndomains:\n- domain: boltic.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/boltic/refs/heads/main/security/boltic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Automation
- Data Sync
- Gateways
- No-Code
- Streaming
- Workflows
---
