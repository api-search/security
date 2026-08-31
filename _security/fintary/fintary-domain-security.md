---
api_specs:
- filename: fintary-agents-api-openapi.yml
  format: yaml
  label: Fintary Agents API
  slug: fintary-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fintary/refs/heads/main/openapi/fintary-agents-api-openapi.yml
- filename: fintary-ams-agents-api-openapi.yml
  format: yaml
  label: Fintary AMS - Agents API
  slug: fintary-ams-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fintary/refs/heads/main/openapi/fintary-ams-agents-api-openapi.yml
- filename: fintary-ams-configs-api-openapi.yml
  format: yaml
  label: Fintary AMS - Configs API
  slug: fintary-ams-configs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fintary/refs/heads/main/openapi/fintary-ams-configs-api-openapi.yml
- filename: fintary-ams-customers-api-openapi.yml
  format: yaml
  label: Fintary AMS - Customers API
  slug: fintary-ams-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fintary/refs/heads/main/openapi/fintary-ams-customers-api-openapi.yml
- filename: fintary-ams-policies-api-openapi.yml
  format: yaml
  label: Fintary AMS - Policies API
  slug: fintary-ams-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fintary/refs/heads/main/openapi/fintary-ams-policies-api-openapi.yml
- filename: fintary-ams-registry-api-openapi.yml
  format: yaml
  label: Fintary AMS - Registry API
  slug: fintary-ams-registry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fintary/refs/heads/main/openapi/fintary-ams-registry-api-openapi.yml
- filename: fintary-ams-tasks-api-openapi.yml
  format: yaml
  label: Fintary AMS - Tasks API
  slug: fintary-ams-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fintary/refs/heads/main/openapi/fintary-ams-tasks-api-openapi.yml
- filename: fintary-analytics-api-openapi.yml
  format: yaml
  label: Fintary Analytics API
  slug: fintary-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fintary/refs/heads/main/openapi/fintary-analytics-api-openapi.yml
- filename: fintary-commission-reports-api-openapi.yml
  format: yaml
  label: Fintary Commission Reports API
  slug: fintary-commission-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fintary/refs/heads/main/openapi/fintary-commission-reports-api-openapi.yml
- filename: fintary-documents-api-openapi.yml
  format: yaml
  label: Fintary Documents API
  slug: fintary-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fintary/refs/heads/main/openapi/fintary-documents-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fintary.com
  spf: true
hosts:
- cert_expires: Oct 14 22:50:08 2026 GMT
  host: fintary.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 11 14:49:55 2026 GMT
  host: api.fintary.com
  hsts: true
  hsts_max_age: 63072000
  hsts_note: 'The mechanical probe records null because HEAD https://api.fintary.com/ returns the Next.js 404 page, which carries no HSTS header. A direct GET of a real API route (https://api.fintary.com/openapi/agents, HTTP 401) on 2026-08-14 returned `strict-transport-security: max-age=63072000; includeSubDomains`.'
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fintary Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fintary, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Fintary
provider_slug: fintary
slug: fintary-domain-security
source_filename: fintary-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fintary.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 22:50:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.fintary.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 14:49:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_note: >-\n    The mechanical probe records null because HEAD https://api.fintary.com/ returns the Next.js\n    404 page, which carries no HSTS header. A direct GET of a real API route\n    (https://api.fintary.com/openapi/agents, HTTP 401) on 2026-08-14 returned\n    `strict-transport-security: max-age=63072000; includeSubDomains`.\ndomains:\n- domain: fintary.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fintary/refs/heads/main/security/fintary-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Insurance
- Insurtech
- Commissions
- Revenue Operations
- Analytics
- Agency Management
- Policy Management
- Payouts
- Reconciliation
- OpenAPI
---
