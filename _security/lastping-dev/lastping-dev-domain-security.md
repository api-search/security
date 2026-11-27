---
api_specs:
- filename: lastping-dev-agents-api-openapi.yml
  format: yaml
  label: LastPing Agents API
  slug: lastping-dev-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lastping-dev/openapi/lastping-dev-agents-api-openapi.yml
- filename: lastping-dev-auth-api-openapi.yml
  format: yaml
  label: LastPing Auth API
  slug: lastping-dev-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lastping-dev/openapi/lastping-dev-auth-api-openapi.yml
- filename: lastping-dev-channels-api-openapi.yml
  format: yaml
  label: LastPing Channels API
  slug: lastping-dev-channels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lastping-dev/openapi/lastping-dev-channels-api-openapi.yml
- filename: lastping-dev-checks-api-openapi.yml
  format: yaml
  label: LastPing Checks API
  slug: lastping-dev-checks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lastping-dev/openapi/lastping-dev-checks-api-openapi.yml
- filename: lastping-dev-ci-api-openapi.yml
  format: yaml
  label: LastPing CI API
  slug: lastping-dev-ci-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lastping-dev/openapi/lastping-dev-ci-api-openapi.yml
- filename: lastping-dev-discovery-api-openapi.yml
  format: yaml
  label: LastPing Discovery API
  slug: lastping-dev-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lastping-dev/openapi/lastping-dev-discovery-api-openapi.yml
- filename: lastping-dev-events-api-openapi.yml
  format: yaml
  label: LastPing Events API
  slug: lastping-dev-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lastping-dev/openapi/lastping-dev-events-api-openapi.yml
- filename: lastping-dev-export-api-openapi.yml
  format: yaml
  label: LastPing Export API
  slug: lastping-dev-export-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lastping-dev/openapi/lastping-dev-export-api-openapi.yml
- filename: lastping-dev-health-api-openapi.yml
  format: yaml
  label: LastPing Health API
  slug: lastping-dev-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lastping-dev/openapi/lastping-dev-health-api-openapi.yml
- filename: lastping-dev-incidents-api-openapi.yml
  format: yaml
  label: LastPing Incidents API
  slug: lastping-dev-incidents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lastping-dev/openapi/lastping-dev-incidents-api-openapi.yml
- filename: lastping-dev-metrics-api-openapi.yml
  format: yaml
  label: LastPing Metrics API
  slug: lastping-dev-metrics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lastping-dev/openapi/lastping-dev-metrics-api-openapi.yml
- filename: lastping-dev-monitors-api-openapi.yml
  format: yaml
  label: LastPing Monitors API
  slug: lastping-dev-monitors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lastping-dev/openapi/lastping-dev-monitors-api-openapi.yml
- filename: lastping-dev-routes-api-openapi.yml
  format: yaml
  label: LastPing Routes API
  slug: lastping-dev-routes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lastping-dev/openapi/lastping-dev-routes-api-openapi.yml
- filename: lastping-dev-statuspages-api-openapi.yml
  format: yaml
  label: LastPing Status Pages API
  slug: lastping-dev-statuspages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lastping-dev/openapi/lastping-dev-statuspages-api-openapi.yml
- filename: lastping-dev-traces-api-openapi.yml
  format: yaml
  label: LastPing Traces API
  slug: lastping-dev-traces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lastping-dev/openapi/lastping-dev-traces-api-openapi.yml
- filename: lastping-dev-api-keys-api-openapi.yml
  format: yaml
  label: LastPing API Keys API
  slug: lastping-dev-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lastping-dev/openapi/lastping-dev-api-keys-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lastping.dev
  spf: true
hosts:
- cert_expires: Apr 23 23:59:59 2027 GMT
  host: lastping.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: LastPing Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LastPing, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: LastPing
provider_slug: lastping-dev
slug: lastping-dev-domain-security
source_filename: lastping-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lastping.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 23 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lastping.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/lastping-dev/security/lastping-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Monitoring
- Artificial Intelligence
- DevOps
- Open Source
- Automation
---
