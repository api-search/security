---
api_specs:
- filename: apuchat-com-channels-api-openapi.yml
  format: yaml
  label: Apuchat Channels API
  slug: apuchat-com-channels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apuchat-com/openapi/apuchat-com-channels-api-openapi.yml
- filename: apuchat-com-healthz-api-openapi.yml
  format: yaml
  label: Apuchat Healthz API
  slug: apuchat-com-healthz-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apuchat-com/openapi/apuchat-com-healthz-api-openapi.yml
- filename: apuchat-com-info-api-openapi.yml
  format: yaml
  label: Apuchat Info API
  slug: apuchat-com-info-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apuchat-com/openapi/apuchat-com-info-api-openapi.yml
- filename: apuchat-com-stats-api-openapi.yml
  format: yaml
  label: Apuchat Stats API
  slug: apuchat-com-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apuchat-com/openapi/apuchat-com-stats-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: apuchat.com
  spf: false
hosts:
- cert_expires: Dec 23 21:56:48 2026 GMT
  host: apuchat.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Apuchat Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apuchat, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Apuchat
provider_slug: apuchat-com
slug: apuchat-com-domain-security
source_filename: apuchat-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apuchat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 21:56:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: apuchat.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/apuchat-com/security/apuchat-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Communications
- Multi-Agent
- MCP
- Chat
---
