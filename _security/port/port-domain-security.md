---
api_specs:
- filename: port-action-runs-api-openapi.yml
  format: yaml
  label: Port Action Runs API
  slug: port-action-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/port/refs/heads/main/openapi/port-action-runs-api-openapi.yml
- filename: port-actions-api-openapi.yml
  format: yaml
  label: Port Actions API
  slug: port-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/port/refs/heads/main/openapi/port-actions-api-openapi.yml
- filename: port-apps-api-openapi.yml
  format: yaml
  label: Port Apps API
  slug: port-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/port/refs/heads/main/openapi/port-apps-api-openapi.yml
- filename: port-audit-api-openapi.yml
  format: yaml
  label: Port Audit API
  slug: port-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/port/refs/heads/main/openapi/port-audit-api-openapi.yml
- filename: port-authentication-authorization-api-openapi.yml
  format: yaml
  label: Port Authentication / Authorization API
  slug: port-authentication-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/port/refs/heads/main/openapi/port-authentication-authorization-api-openapi.yml
- filename: port-blueprints-api-openapi.yml
  format: yaml
  label: Port Blueprints API
  slug: port-blueprints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/port/refs/heads/main/openapi/port-blueprints-api-openapi.yml
- filename: port-entities-api-openapi.yml
  format: yaml
  label: Port Entities API
  slug: port-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/port/refs/heads/main/openapi/port-entities-api-openapi.yml
- filename: port-integrations-api-openapi.yml
  format: yaml
  label: Port Integrations API
  slug: port-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/port/refs/heads/main/openapi/port-integrations-api-openapi.yml
- filename: port-migrations-api-openapi.yml
  format: yaml
  label: Port Migrations API
  slug: port-migrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/port/refs/heads/main/openapi/port-migrations-api-openapi.yml
- filename: port-organization-api-openapi.yml
  format: yaml
  label: Port Organization API
  slug: port-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/port/refs/heads/main/openapi/port-organization-api-openapi.yml
- filename: port-pages-api-openapi.yml
  format: yaml
  label: Port Pages API
  slug: port-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/port/refs/heads/main/openapi/port-pages-api-openapi.yml
- filename: port-scorecards-api-openapi.yml
  format: yaml
  label: Port Scorecards API
  slug: port-scorecards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/port/refs/heads/main/openapi/port-scorecards-api-openapi.yml
- filename: port-teams-api-openapi.yml
  format: yaml
  label: Port Teams API
  slug: port-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/port/refs/heads/main/openapi/port-teams-api-openapi.yml
- filename: port-users-api-openapi.yml
  format: yaml
  label: Port Users API
  slug: port-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/port/refs/heads/main/openapi/port-users-api-openapi.yml
- filename: port-webhook-api-openapi.yml
  format: yaml
  label: Port Webhook API
  slug: port-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/port/refs/heads/main/openapi/port-webhook-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: port.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: getport.io
  spf: true
hosts:
- cert_expires: Sep 19 15:41:46 2026 GMT
  host: www.port.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  3 23:59:59 2027 GMT
  host: docs.getport.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 21 23:59:59 2027 GMT
  host: api.getport.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Port Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Port, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Port
provider_slug: port
slug: port-domain-security
source_filename: port-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.port.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 15:41:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.getport.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 23:59:59 2027 GMT\n  hsts: false\n- host: api.getport.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: port.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: getport.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/port/refs/heads/main/security/port-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Automations
- Developer Portals
- Internal Developer Portal
- Platform Engineering
- Scorecards
- Self-Service
- Software Catalog
---
