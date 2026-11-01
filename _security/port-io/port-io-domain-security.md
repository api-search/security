---
api_specs:
- filename: port-io-blueprints-api-openapi.yml
  format: yaml
  label: Port Blueprints API
  slug: port-io-blueprints-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/port-io/openapi/port-io-blueprints-api-openapi.yml
- filename: port-io-entities-api-openapi.yml
  format: yaml
  label: Port Entities API
  slug: port-io-entities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/port-io/openapi/port-io-entities-api-openapi.yml
- filename: port-io-action-runs-api-openapi.yml
  format: yaml
  label: Port Action Runs API
  slug: port-io-action-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/port-io/openapi/port-io-action-runs-api-openapi.yml
- filename: port-io-actions-api-openapi.yml
  format: yaml
  label: Port Actions API
  slug: port-io-actions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/port-io/openapi/port-io-actions-api-openapi.yml
- filename: port-io-ai-api-openapi.yml
  format: yaml
  label: Port AI API
  slug: port-io-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/port-io/openapi/port-io-ai-api-openapi.yml
- filename: port-io-apps-api-openapi.yml
  format: yaml
  label: Port Apps API
  slug: port-io-apps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/port-io/openapi/port-io-apps-api-openapi.yml
- filename: port-io-audit-api-openapi.yml
  format: yaml
  label: Port Audit API
  slug: port-io-audit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/port-io/openapi/port-io-audit-api-openapi.yml
- filename: port-io-authentication-authorization-api-openapi.yml
  format: yaml
  label: Port Authentication / Authorization API
  slug: port-io-authentication-authorization-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/port-io/openapi/port-io-authentication-authorization-api-openapi.yml
- filename: port-io-folders-api-openapi.yml
  format: yaml
  label: Port Folders API
  slug: port-io-folders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/port-io/openapi/port-io-folders-api-openapi.yml
- filename: port-io-integrations-api-openapi.yml
  format: yaml
  label: Port Integrations API
  slug: port-io-integrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/port-io/openapi/port-io-integrations-api-openapi.yml
- filename: port-io-migrations-api-openapi.yml
  format: yaml
  label: Port Migrations API
  slug: port-io-migrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/port-io/openapi/port-io-migrations-api-openapi.yml
- filename: port-io-organization-api-openapi.yml
  format: yaml
  label: Port Organization API
  slug: port-io-organization-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/port-io/openapi/port-io-organization-api-openapi.yml
- filename: port-io-pages-api-openapi.yml
  format: yaml
  label: Port Pages API
  slug: port-io-pages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/port-io/openapi/port-io-pages-api-openapi.yml
- filename: port-io-scorecard-groups-api-openapi.yml
  format: yaml
  label: Port Scorecard Groups API
  slug: port-io-scorecard-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/port-io/openapi/port-io-scorecard-groups-api-openapi.yml
- filename: port-io-scorecards-api-openapi.yml
  format: yaml
  label: Port Scorecards API
  slug: port-io-scorecards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/port-io/openapi/port-io-scorecards-api-openapi.yml
- filename: port-io-teams-api-openapi.yml
  format: yaml
  label: Port Teams API
  slug: port-io-teams-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/port-io/openapi/port-io-teams-api-openapi.yml
- filename: port-io-users-api-openapi.yml
  format: yaml
  label: Port Users API
  slug: port-io-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/port-io/openapi/port-io-users-api-openapi.yml
- filename: port-io-webhook-api-openapi.yml
  format: yaml
  label: Port Webhook API
  slug: port-io-webhook-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/port-io/openapi/port-io-webhook-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: port.io
  spf: true
hosts:
- cert_expires: Sep 19 15:41:46 2026 GMT
  host: www.port.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 30 23:59:59 2026 GMT
  host: docs.port.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 22 23:59:59 2027 GMT
  host: api.port.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Port Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Port, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Port
provider_slug: port-io
slug: port-io-domain-security
source_filename: port-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.port.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 15:41:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.port.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 23:59:59 2026 GMT\n  hsts: false\n- host: api.port.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 22 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: port.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/port-io/security/port-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Internal Developer Portal
- Service Catalog
- Self-Service Actions
- Platform Engineering
- Scorecards
- Developer Experience
- Developer Portal
---
