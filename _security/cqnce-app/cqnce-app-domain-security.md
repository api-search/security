---
api_specs:
- filename: cqnce-app-agents-admin-api-openapi.yml
  format: yaml
  label: cQnce Agents – Admin API
  slug: cqnce-app-agents-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cqnce-app/openapi/cqnce-app-agents-admin-api-openapi.yml
- filename: cqnce-app-agents-self-api-openapi.yml
  format: yaml
  label: cQnce Agents – Self API
  slug: cqnce-app-agents-self-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cqnce-app/openapi/cqnce-app-agents-self-api-openapi.yml
- filename: cqnce-app-alarms-api-openapi.yml
  format: yaml
  label: cQnce Alarms API
  slug: cqnce-app-alarms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cqnce-app/openapi/cqnce-app-alarms-api-openapi.yml
- filename: cqnce-app-auth-agent-api-openapi.yml
  format: yaml
  label: cQnce Auth – Agent API
  slug: cqnce-app-auth-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cqnce-app/openapi/cqnce-app-auth-agent-api-openapi.yml
- filename: cqnce-app-auth-tenant-api-openapi.yml
  format: yaml
  label: cQnce Auth – Tenant API
  slug: cqnce-app-auth-tenant-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cqnce-app/openapi/cqnce-app-auth-tenant-api-openapi.yml
- filename: cqnce-app-callbacks-api-openapi.yml
  format: yaml
  label: cQnce Callbacks API
  slug: cqnce-app-callbacks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cqnce-app/openapi/cqnce-app-callbacks-api-openapi.yml
- filename: cqnce-app-health-api-openapi.yml
  format: yaml
  label: cQnce Health API
  slug: cqnce-app-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cqnce-app/openapi/cqnce-app-health-api-openapi.yml
- filename: cqnce-app-logs-api-openapi.yml
  format: yaml
  label: cQnce Logs API
  slug: cqnce-app-logs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cqnce-app/openapi/cqnce-app-logs-api-openapi.yml
- filename: cqnce-app-projects-api-openapi.yml
  format: yaml
  label: cQnce Projects API
  slug: cqnce-app-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cqnce-app/openapi/cqnce-app-projects-api-openapi.yml
- filename: cqnce-app-public-api-openapi.yml
  format: yaml
  label: cQnce Public API
  slug: cqnce-app-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cqnce-app/openapi/cqnce-app-public-api-openapi.yml
- filename: cqnce-app-requests-api-openapi.yml
  format: yaml
  label: cQnce Requests API
  slug: cqnce-app-requests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cqnce-app/openapi/cqnce-app-requests-api-openapi.yml
- filename: cqnce-app-routing-rules-api-openapi.yml
  format: yaml
  label: cQnce Routing Rules API
  slug: cqnce-app-routing-rules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cqnce-app/openapi/cqnce-app-routing-rules-api-openapi.yml
- filename: cqnce-app-subscriptions-api-openapi.yml
  format: yaml
  label: cQnce Subscriptions API
  slug: cqnce-app-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cqnce-app/openapi/cqnce-app-subscriptions-api-openapi.yml
- filename: cqnce-app-teams-api-openapi.yml
  format: yaml
  label: cQnce Teams API
  slug: cqnce-app-teams-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cqnce-app/openapi/cqnce-app-teams-api-openapi.yml
- filename: cqnce-app-users-api-openapi.yml
  format: yaml
  label: cQnce Users API
  slug: cqnce-app-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cqnce-app/openapi/cqnce-app-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cqnce.app
  spf: true
hosts:
- cert_expires: Jan 22 13:58:05 2027 GMT
  host: cqnce.app
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 22 13:58:05 2027 GMT
  host: api.cqnce.app
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: cQnce Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for cQnce, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: cQnce
provider_slug: cqnce-app
slug: cqnce-app-domain-security
source_filename: cqnce-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cqnce.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 13:58:05 2027 GMT\n  hsts: false\n- host: api.cqnce.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 13:58:05 2027 GMT\n  hsts: null\ndomains:\n- domain: cqnce.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/cqnce-app/security/cqnce-app-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Human-in-the-Loop
- Approvals
- Authorization
- AI Agents
- MCP
- Webhook
- Workflows
- Audit
---
