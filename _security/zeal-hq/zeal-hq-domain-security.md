---
api_specs:
- filename: zeal-hq-openapi.yml
  format: yaml
  label: Zeal Companies API
  slug: zeal-hq-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeal-hq/refs/heads/main/openapi/zeal-hq-openapi.yml
- filename: zeal-hq-openapi.yml
  format: yaml
  label: Zeal Employees API
  slug: zeal-hq-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeal-hq/refs/heads/main/openapi/zeal-hq-openapi.yml
- filename: zeal-hq-openapi.yml
  format: yaml
  label: Zeal Contractors API
  slug: zeal-hq-contractors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeal-hq/refs/heads/main/openapi/zeal-hq-openapi.yml
- filename: zeal-hq-openapi.yml
  format: yaml
  label: Zeal Employee Check (Payroll Run) API
  slug: zeal-hq-employee-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeal-hq/refs/heads/main/openapi/zeal-hq-openapi.yml
- filename: zeal-hq-openapi.yml
  format: yaml
  label: Zeal Contractor Payments API
  slug: zeal-hq-contractor-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeal-hq/refs/heads/main/openapi/zeal-hq-openapi.yml
- filename: zeal-hq-openapi.yml
  format: yaml
  label: Zeal Pay Schedules API
  slug: zeal-hq-pay-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeal-hq/refs/heads/main/openapi/zeal-hq-openapi.yml
- filename: zeal-hq-openapi.yml
  format: yaml
  label: Zeal Worker Onboarding API
  slug: zeal-hq-onboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeal-hq/refs/heads/main/openapi/zeal-hq-openapi.yml
- filename: zeal-hq-openapi.yml
  format: yaml
  label: Zeal Tax and Compliance API
  slug: zeal-hq-tax-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeal-hq/refs/heads/main/openapi/zeal-hq-openapi.yml
- filename: zeal-hq-openapi.yml
  format: yaml
  label: Zeal Reports API
  slug: zeal-hq-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeal-hq/refs/heads/main/openapi/zeal-hq-openapi.yml
- filename: zeal-hq-openapi.yml
  format: yaml
  label: Zeal Funding and Journal API
  slug: zeal-hq-funding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeal-hq/refs/heads/main/openapi/zeal-hq-openapi.yml
- filename: zeal-hq-openapi.yml
  format: yaml
  label: Zeal Webhooks and Events API
  slug: zeal-hq-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeal-hq/refs/heads/main/openapi/zeal-hq-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: zeal.com
  spf: true
hosts:
- cert_expires: Sep 22 18:29:28 2026 GMT
  host: www.zeal.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 19:22:43 2026 GMT
  host: docs.zeal.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 18 23:59:59 2026 GMT
  host: api.zeal.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Zeal Hq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zeal, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Zeal
provider_slug: zeal-hq
slug: zeal-hq-domain-security
source_filename: zeal-hq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zeal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 18:29:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.zeal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 19:22:43 2026 GMT\n  hsts: null\n- host: api.zeal.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 18 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: zeal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zeal-hq/refs/heads/main/security/zeal-hq-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payroll
- Embedded Finance
- Fintech
- Tax Compliance
- Contractors
- Human Resources
---
