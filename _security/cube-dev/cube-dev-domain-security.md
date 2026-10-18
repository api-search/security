---
api_specs:
- filename: cube-dev-audit-logs-api-openapi.yml
  format: yaml
  label: Cube Dev Audit Logs API
  slug: cube-dev-audit-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cube-dev/refs/heads/main/openapi/cube-dev-audit-logs-api-openapi.yml
- filename: cube-dev-build-api-openapi.yml
  format: yaml
  label: Cube Dev Build API
  slug: cube-dev-build-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cube-dev/refs/heads/main/openapi/cube-dev-build-api-openapi.yml
- filename: cube-dev-cube-dev-api-api-openapi.yml
  format: yaml
  label: Cube Dev Cube Dev API
  slug: cube-dev-cube-dev-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cube-dev/refs/heads/main/openapi/cube-dev-cube-dev-api-api-openapi.yml
- filename: cube-dev-cube-js-api-openapi.yml
  format: yaml
  label: Cube Dev Cube Js API
  slug: cube-dev-cube-js-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cube-dev/refs/heads/main/openapi/cube-dev-cube-js-api-openapi.yml
- filename: cube-dev-cubejs-api-api-openapi.yml
  format: yaml
  label: Cube Dev Cubejs API
  slug: cube-dev-cubejs-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cube-dev/refs/heads/main/openapi/cube-dev-cubejs-api-api-openapi.yml
- filename: cube-dev-dashboard-api-openapi.yml
  format: yaml
  label: Cube Dev Dashboard API
  slug: cube-dev-dashboard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cube-dev/refs/heads/main/openapi/cube-dev-dashboard-api-openapi.yml
- filename: cube-dev-deployments-api-openapi.yml
  format: yaml
  label: Cube Dev Deployments API
  slug: cube-dev-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cube-dev/refs/heads/main/openapi/cube-dev-deployments-api-openapi.yml
- filename: cube-dev-embed-api-openapi.yml
  format: yaml
  label: Cube Dev Embed API
  slug: cube-dev-embed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cube-dev/refs/heads/main/openapi/cube-dev-embed-api-openapi.yml
- filename: cube-dev-embed-tenants-api-openapi.yml
  format: yaml
  label: Cube Dev Embed Tenants API
  slug: cube-dev-embed-tenants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cube-dev/refs/heads/main/openapi/cube-dev-embed-tenants-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: cube.dev
  spf: true
hosts:
- cert_expires: Jan 12 23:59:59 2027 GMT
  host: cube.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cube Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cube Dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Cube Dev
provider_slug: cube-dev
slug: cube-dev-domain-security
source_filename: cube-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cube.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cube.dev\n  dnssec: true\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cube-dev/refs/heads/main/security/cube-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Analytics
- Artificial Intelligence
- Business-Intelligence
- Platform
---
