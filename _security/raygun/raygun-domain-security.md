---
api_specs:
- filename: raygun-applications-api-openapi.yml
  format: yaml
  label: Raygun Applications API
  slug: raygun-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/raygun/refs/heads/main/openapi/raygun-applications-api-openapi.yml
- filename: raygun-errors-api-openapi.yml
  format: yaml
  label: Raygun Errors API
  slug: raygun-errors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/raygun/refs/heads/main/openapi/raygun-errors-api-openapi.yml
- filename: raygun-deployments-api-openapi.yml
  format: yaml
  label: Raygun Deployments API
  slug: raygun-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/raygun/refs/heads/main/openapi/raygun-deployments-api-openapi.yml
- filename: raygun-source-maps-api-openapi.yml
  format: yaml
  label: Raygun Source Maps API
  slug: raygun-source-maps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/raygun/refs/heads/main/openapi/raygun-source-maps-api-openapi.yml
- filename: raygun-sessions-api-openapi.yml
  format: yaml
  label: Raygun Sessions API
  slug: raygun-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/raygun/refs/heads/main/openapi/raygun-sessions-api-openapi.yml
- filename: raygun-pages-api-openapi.yml
  format: yaml
  label: Raygun Pages API
  slug: raygun-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/raygun/refs/heads/main/openapi/raygun-pages-api-openapi.yml
- filename: raygun-customers-api-openapi.yml
  format: yaml
  label: Raygun Customers API
  slug: raygun-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/raygun/refs/heads/main/openapi/raygun-customers-api-openapi.yml
- filename: raygun-metrics-api-openapi.yml
  format: yaml
  label: Raygun Metrics API
  slug: raygun-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/raygun/refs/heads/main/openapi/raygun-metrics-api-openapi.yml
- filename: raygun-flutter-symbols-api-openapi.yml
  format: yaml
  label: Raygun Flutter Symbols API
  slug: raygun-flutter-symbols-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/raygun/refs/heads/main/openapi/raygun-flutter-symbols-api-openapi.yml
- filename: raygun-teams-api-openapi.yml
  format: yaml
  label: Raygun Teams API
  slug: raygun-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/raygun/refs/heads/main/openapi/raygun-teams-api-openapi.yml
- filename: raygun-invitations-api-openapi.yml
  format: yaml
  label: Raygun Invitations API
  slug: raygun-invitations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/raygun/refs/heads/main/openapi/raygun-invitations-api-openapi.yml
- filename: raygun-plans-api-openapi.yml
  format: yaml
  label: Raygun Plans API
  slug: raygun-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/raygun/refs/heads/main/openapi/raygun-plans-api-openapi.yml
- filename: raygun-webhooks-asyncapi.yml
  format: yaml
  label: Raygun Outbound Webhooks
  slug: raygun-webhooks-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/raygun/refs/heads/main/openapi/raygun-webhooks-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: raygun.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: raygun.io
  spf: true
hosts:
- cert_expires: Jan  3 23:59:59 2027 GMT
  host: raygun.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 26 23:59:59 2026 GMT
  host: api.raygun.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  3 23:59:59 2027 GMT
  host: api.raygun.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Raygun Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Raygun, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Raygun
provider_slug: raygun
slug: raygun-domain-security
source_filename: raygun-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: raygun.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.raygun.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 23:59:59 2026 GMT\n  hsts: null\n- host: api.raygun.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: raygun.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: raygun.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/raygun/refs/heads/main/security/raygun-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Observability
- Crash Reporting
- Real User Monitoring
- Application Performance Monitoring
- Error Tracking
- Errors
- Monitoring
- DevOps
- Source Maps
- Deployments
---
