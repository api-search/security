---
api_specs:
- filename: cms-api-reference-api-openapi.yml
  format: yaml
  label: Centers for Medicare and Medicaid Services API Reference API
  slug: cms-api-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms/refs/heads/main/openapi/cms-api-reference-api-openapi.yml
- filename: cms-bulk-data-api-openapi.yml
  format: yaml
  label: Centers for Medicare and Medicaid Services Bulk Data API
  slug: cms-bulk-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms/refs/heads/main/openapi/cms-bulk-data-api-openapi.yml
- filename: cms-code-search-api-openapi.yml
  format: yaml
  label: Centers for Medicare and Medicaid Services Code Search API
  slug: cms-code-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms/refs/heads/main/openapi/cms-code-search-api-openapi.yml
- filename: cms-cost-search-api-openapi.yml
  format: yaml
  label: Centers for Medicare and Medicaid Services Cost Search API
  slug: cms-cost-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms/refs/heads/main/openapi/cms-cost-search-api-openapi.yml
- filename: cms-enrollments-api-openapi.yml
  format: yaml
  label: Centers for Medicare and Medicaid Services Enrollments API
  slug: cms-enrollments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms/refs/heads/main/openapi/cms-enrollments-api-openapi.yml
- filename: cms-geography-api-openapi.yml
  format: yaml
  label: Centers for Medicare and Medicaid Services Geography API
  slug: cms-geography-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms/refs/heads/main/openapi/cms-geography-api-openapi.yml
- filename: cms-households-eligibility-api-openapi.yml
  format: yaml
  label: Centers for Medicare and Medicaid Services Households & Eligibility API
  slug: cms-households-eligibility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms/refs/heads/main/openapi/cms-households-eligibility-api-openapi.yml
- filename: cms-insurance-issuers-api-openapi.yml
  format: yaml
  label: Centers for Medicare and Medicaid Services Insurance Issuers API
  slug: cms-insurance-issuers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms/refs/heads/main/openapi/cms-insurance-issuers-api-openapi.yml
- filename: cms-insurance-plans-api-openapi.yml
  format: yaml
  label: Centers for Medicare and Medicaid Services Insurance Plans API
  slug: cms-insurance-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms/refs/heads/main/openapi/cms-insurance-plans-api-openapi.yml
- filename: cms-plans-api-openapi.yml
  format: yaml
  label: Centers for Medicare and Medicaid Services Plans API
  slug: cms-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms/refs/heads/main/openapi/cms-plans-api-openapi.yml
- filename: cms-provider-drug-coverage-api-openapi.yml
  format: yaml
  label: Centers for Medicare and Medicaid Services Provider & Drug Coverage API
  slug: cms-provider-drug-coverage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms/refs/heads/main/openapi/cms-provider-drug-coverage-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: cms.gov
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: healthcare.gov
  spf: true
hosts:
- cert_expires: Dec 21 23:59:59 2026 GMT
  host: developer.cms.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 21 23:59:59 2026 GMT
  host: marketplace.api.healthcare.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 22 23:59:59 2027 GMT
  host: bluebutton.cms.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cms Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Centers for Medicare and Medicaid Services, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Centers for Medicare and Medicaid Services
provider_slug: cms
slug: cms-domain-security
source_filename: cms-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.cms.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: marketplace.api.healthcare.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 23:59:59 2026 GMT\n  hsts: null\n- host: bluebutton.cms.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cms.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: healthcare.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cms/refs/heads/main/security/cms-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Medicare
- Medicaid
- Healthcare
- Health Insurance
- FHIR
- Federal Government
- Drug Spending
- Provider Data
- Quality Measures
- Claims Data
---
