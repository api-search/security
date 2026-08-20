---
api_specs:
- filename: humaans-io-audit-events-api-openapi.yml
  format: yaml
  label: Humaans Audit Events API
  slug: humaans-io-audit-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humaans-io/refs/heads/main/openapi/humaans-io-audit-events-api-openapi.yml
- filename: humaans-io-bank-accounts-api-openapi.yml
  format: yaml
  label: Humaans Bank Accounts API
  slug: humaans-io-bank-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humaans-io/refs/heads/main/openapi/humaans-io-bank-accounts-api-openapi.yml
- filename: humaans-io-companies-api-openapi.yml
  format: yaml
  label: Humaans Companies API
  slug: humaans-io-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humaans-io/refs/heads/main/openapi/humaans-io-companies-api-openapi.yml
- filename: humaans-io-compensations-api-openapi.yml
  format: yaml
  label: Humaans Compensations API
  slug: humaans-io-compensations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humaans-io/refs/heads/main/openapi/humaans-io-compensations-api-openapi.yml
- filename: humaans-io-custom-fields-api-openapi.yml
  format: yaml
  label: Humaans Custom Fields API
  slug: humaans-io-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humaans-io/refs/heads/main/openapi/humaans-io-custom-fields-api-openapi.yml
- filename: humaans-io-documents-api-openapi.yml
  format: yaml
  label: Humaans Documents API
  slug: humaans-io-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humaans-io/refs/heads/main/openapi/humaans-io-documents-api-openapi.yml
- filename: humaans-io-equipment-api-openapi.yml
  format: yaml
  label: Humaans Equipment API
  slug: humaans-io-equipment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humaans-io/refs/heads/main/openapi/humaans-io-equipment-api-openapi.yml
- filename: humaans-io-job-roles-api-openapi.yml
  format: yaml
  label: Humaans Job Roles API
  slug: humaans-io-job-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humaans-io/refs/heads/main/openapi/humaans-io-job-roles-api-openapi.yml
- filename: humaans-io-locations-api-openapi.yml
  format: yaml
  label: Humaans Locations API
  slug: humaans-io-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humaans-io/refs/heads/main/openapi/humaans-io-locations-api-openapi.yml
- filename: humaans-io-people-api-openapi.yml
  format: yaml
  label: Humaans People API
  slug: humaans-io-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humaans-io/refs/heads/main/openapi/humaans-io-people-api-openapi.yml
- filename: humaans-io-performance-api-openapi.yml
  format: yaml
  label: Humaans Performance API
  slug: humaans-io-performance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humaans-io/refs/heads/main/openapi/humaans-io-performance-api-openapi.yml
- filename: humaans-io-time-away-api-openapi.yml
  format: yaml
  label: Humaans Time Away API
  slug: humaans-io-time-away-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humaans-io/refs/heads/main/openapi/humaans-io-time-away-api-openapi.yml
- filename: humaans-io-timesheet-api-openapi.yml
  format: yaml
  label: Humaans Timesheet API
  slug: humaans-io-timesheet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humaans-io/refs/heads/main/openapi/humaans-io-timesheet-api-openapi.yml
- filename: humaans-io-webhooks-api-openapi.yml
  format: yaml
  label: Humaans Webhooks API
  slug: humaans-io-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humaans-io/refs/heads/main/openapi/humaans-io-webhooks-api-openapi.yml
- filename: humaans-io-working-patterns-api-openapi.yml
  format: yaml
  label: Humaans Working Patterns API
  slug: humaans-io-working-patterns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humaans-io/refs/heads/main/openapi/humaans-io-working-patterns-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: humaans.io
  spf: true
hosts:
- cert_expires: Aug 25 13:23:52 2026 GMT
  host: humaans.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 17:53:42 2026 GMT
  host: docs.humaans.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 18:14:44 2026 GMT
  host: app.humaans.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Humaans Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Humaans, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Humaans
provider_slug: humaans-io
slug: humaans-io-domain-security
source_filename: humaans-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: humaans.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 13:23:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.humaans.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 17:53:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.humaans.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 18:14:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: humaans.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/humaans-io/refs/heads/main/security/humaans-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- HR
- HRIS
- Human Resources
- People Operations
- People Analytics
- Onboarding
- Offboarding
- Performance Management
- Time Off
- Compensation
- Workflow-Automation
- AI Companion
- Agentic AI
- UK
- London
---
