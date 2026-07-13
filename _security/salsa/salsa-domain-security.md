---
api_specs:
- filename: salsa-openapi.yml
  format: yaml
  label: Salsa Companies API
  slug: salsa-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salsa/refs/heads/main/openapi/salsa-openapi.yml
- filename: salsa-openapi.yml
  format: yaml
  label: Salsa Workers API
  slug: salsa-workers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salsa/refs/heads/main/openapi/salsa-openapi.yml
- filename: salsa-openapi.yml
  format: yaml
  label: Salsa Pay Schedules API
  slug: salsa-pay-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salsa/refs/heads/main/openapi/salsa-openapi.yml
- filename: salsa-openapi.yml
  format: yaml
  label: Salsa Payrolls API
  slug: salsa-payrolls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salsa/refs/heads/main/openapi/salsa-openapi.yml
- filename: salsa-openapi.yml
  format: yaml
  label: Salsa Payments API
  slug: salsa-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salsa/refs/heads/main/openapi/salsa-openapi.yml
- filename: salsa-openapi.yml
  format: yaml
  label: Salsa Onboarding & Sessions API
  slug: salsa-onboarding-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salsa/refs/heads/main/openapi/salsa-openapi.yml
- filename: salsa-openapi.yml
  format: yaml
  label: Salsa Tax API
  slug: salsa-tax-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salsa/refs/heads/main/openapi/salsa-openapi.yml
- filename: salsa-openapi.yml
  format: yaml
  label: Salsa Webhooks API
  slug: salsa-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salsa/refs/heads/main/openapi/salsa-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: salsa.dev
  spf: true
hosts:
- cert_expires: Aug 16 16:44:21 2026 GMT
  host: www.salsa.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 07:12:19 2026 GMT
  host: docs.salsa.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  3 23:59:59 2026 GMT
  host: api.salsa.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Salsa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Salsa, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Salsa
provider_slug: salsa
slug: salsa-domain-security
source_filename: salsa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.salsa.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 16:44:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.salsa.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 07:12:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.salsa.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  3 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: salsa.dev\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/salsa/refs/heads/main/security/salsa-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Payroll
- Embedded Finance
- Payroll as a Service
- Fintech
- Payments
- HR
- Tax
- Multi-Country
---
