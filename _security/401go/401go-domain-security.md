---
api_specs:
- filename: 401go-affiliates-firms-api-openapi.yml
  format: yaml
  label: 401GO Affiliates & Firms API
  slug: 401go-affiliates-firms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/401go/refs/heads/main/openapi/401go-affiliates-firms-api-openapi.yml
- filename: 401go-beneficiaries-api-openapi.yml
  format: yaml
  label: 401GO Beneficiaries API
  slug: 401go-beneficiaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/401go/refs/heads/main/openapi/401go-beneficiaries-api-openapi.yml
- filename: 401go-companies-plans-api-openapi.yml
  format: yaml
  label: 401GO Companies & Plans API
  slug: 401go-companies-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/401go/refs/heads/main/openapi/401go-companies-plans-api-openapi.yml
- filename: 401go-contributions-payroll-api-openapi.yml
  format: yaml
  label: 401GO Contributions & Payroll API
  slug: 401go-contributions-payroll-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/401go/refs/heads/main/openapi/401go-contributions-payroll-api-openapi.yml
- filename: 401go-documents-api-openapi.yml
  format: yaml
  label: 401GO Documents API
  slug: 401go-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/401go/refs/heads/main/openapi/401go-documents-api-openapi.yml
- filename: 401go-investments-portfolios-api-openapi.yml
  format: yaml
  label: 401GO Investments & Portfolios API
  slug: 401go-investments-portfolios-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/401go/refs/heads/main/openapi/401go-investments-portfolios-api-openapi.yml
- filename: 401go-money-movement-api-openapi.yml
  format: yaml
  label: 401GO Money Movement API
  slug: 401go-money-movement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/401go/refs/heads/main/openapi/401go-money-movement-api-openapi.yml
- filename: 401go-notifications-api-openapi.yml
  format: yaml
  label: 401GO Notifications API
  slug: 401go-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/401go/refs/heads/main/openapi/401go-notifications-api-openapi.yml
- filename: 401go-participants-api-openapi.yml
  format: yaml
  label: 401GO Participants API
  slug: 401go-participants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/401go/refs/heads/main/openapi/401go-participants-api-openapi.yml
- filename: 401go-retirement-planning-api-openapi.yml
  format: yaml
  label: 401GO Retirement Planning API
  slug: 401go-retirement-planning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/401go/refs/heads/main/openapi/401go-retirement-planning-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: 401go.com
  spf: true
hosts:
- cert_expires: Oct  6 06:17:38 2026 GMT
  host: 401go.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 12:59:59 2026 GMT
  host: developer.401go.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 19 08:00:17 2026 GMT
  host: app.401go.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 401Go Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 401GO, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: 401GO
provider_slug: 401go
slug: 401go-domain-security
source_filename: 401go-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 401go.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 06:17:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.401go.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 12:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.401go.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 08:00:17 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: 401go.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/401go/refs/heads/main/security/401go-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Retirement
- 401k
- Financial Services
- Fintech
- Payroll
- Human Resources
- Benefits
- Investments
- Wealth Management
---
