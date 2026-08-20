---
api_specs:
- filename: lendapi-amortization-api-openapi.yml
  format: yaml
  label: LendAPI Amortization API
  slug: lendapi-amortization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendapi/refs/heads/main/openapi/lendapi-amortization-api-openapi.yml
- filename: lendapi-application-api-openapi.yml
  format: yaml
  label: LendAPI Application API
  slug: lendapi-application-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendapi/refs/heads/main/openapi/lendapi-application-api-openapi.yml
- filename: lendapi-credit-risk-api-openapi.yml
  format: yaml
  label: LendAPI Credit Risk API
  slug: lendapi-credit-risk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendapi/refs/heads/main/openapi/lendapi-credit-risk-api-openapi.yml
- filename: lendapi-decision-api-openapi.yml
  format: yaml
  label: LendAPI Decision API
  slug: lendapi-decision-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendapi/refs/heads/main/openapi/lendapi-decision-api-openapi.yml
- filename: lendapi-decisions-api-openapi.yml
  format: yaml
  label: LendAPI Decisions API
  slug: lendapi-decisions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendapi/refs/heads/main/openapi/lendapi-decisions-api-openapi.yml
- filename: lendapi-get-app-credit-report-api-openapi.yml
  format: yaml
  label: LendAPI Get App Credit Report API
  slug: lendapi-get-app-credit-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendapi/refs/heads/main/openapi/lendapi-get-app-credit-report-api-openapi.yml
- filename: lendapi-outcomes-api-openapi.yml
  format: yaml
  label: LendAPI Outcomes API
  slug: lendapi-outcomes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendapi/refs/heads/main/openapi/lendapi-outcomes-api-openapi.yml
- filename: lendapi-page-submit-api-openapi.yml
  format: yaml
  label: LendAPI Page Submit API
  slug: lendapi-page-submit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendapi/refs/heads/main/openapi/lendapi-page-submit-api-openapi.yml
- filename: lendapi-pricing-engine-api-openapi.yml
  format: yaml
  label: LendAPI Pricing Engine API
  slug: lendapi-pricing-engine-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendapi/refs/heads/main/openapi/lendapi-pricing-engine-api-openapi.yml
- filename: lendapi-pricing-engines-api-openapi.yml
  format: yaml
  label: LendAPI Pricing Engines API
  slug: lendapi-pricing-engines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendapi/refs/heads/main/openapi/lendapi-pricing-engines-api-openapi.yml
- filename: lendapi-sub-tenant-api-openapi.yml
  format: yaml
  label: LendAPI Sub Tenant API
  slug: lendapi-sub-tenant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendapi/refs/heads/main/openapi/lendapi-sub-tenant-api-openapi.yml
- filename: lendapi-sub-tenants-api-openapi.yml
  format: yaml
  label: LendAPI Sub Tenants API
  slug: lendapi-sub-tenants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendapi/refs/heads/main/openapi/lendapi-sub-tenants-api-openapi.yml
- filename: lendapi-variable-api-openapi.yml
  format: yaml
  label: LendAPI Variable API
  slug: lendapi-variable-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendapi/refs/heads/main/openapi/lendapi-variable-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lendapi.com
  spf: true
hosts:
- cert_expires: Oct  2 11:56:38 2026 GMT
  host: lendapi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 24 23:59:59 2026 GMT
  host: app.lendapi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lendapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LendAPI, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: LendAPI
provider_slug: lendapi
slug: lendapi-domain-security
source_filename: lendapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lendapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 11:56:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.lendapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lendapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lendapi/refs/heads/main/security/lendapi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Lending
- Loan Origination
- Financial-Services
- Fintech
- Embedded Finance
- Underwriting
- Decision Engine
- Credit
- Banking
- Account Opening
- KYC
- KYB
- Buy Now Pay Later
- Point-of-Sale
---
