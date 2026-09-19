---
api_specs:
- filename: workday-benefits-benefit-enrollments-api-openapi.yml
  format: yaml
  label: Workday Benefits Benefit Enrollments API
  slug: workday-benefits-benefit-enrollments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-benefits/refs/heads/main/openapi/workday-benefits-benefit-enrollments-api-openapi.yml
- filename: workday-benefits-benefit-events-api-openapi.yml
  format: yaml
  label: Workday Benefits Benefit Events API
  slug: workday-benefits-benefit-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-benefits/refs/heads/main/openapi/workday-benefits-benefit-events-api-openapi.yml
- filename: workday-benefits-benefit-plans-api-openapi.yml
  format: yaml
  label: Workday Benefits Benefit Plans API
  slug: workday-benefits-benefit-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-benefits/refs/heads/main/openapi/workday-benefits-benefit-plans-api-openapi.yml
- filename: workday-benefits-dependents-api-openapi.yml
  format: yaml
  label: Workday Benefits Dependents API
  slug: workday-benefits-dependents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-benefits/refs/heads/main/openapi/workday-benefits-dependents-api-openapi.yml
- filename: workday-benefits-employee-benefits-api-openapi.yml
  format: yaml
  label: Workday Benefits Employee Benefits API
  slug: workday-benefits-employee-benefits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-benefits/refs/heads/main/openapi/workday-benefits-employee-benefits-api-openapi.yml
- filename: workday-benefits-time-off-plans-api-openapi.yml
  format: yaml
  label: Workday Benefits Time Off Plans API
  slug: workday-benefits-time-off-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-benefits/refs/heads/main/openapi/workday-benefits-time-off-plans-api-openapi.yml
- filename: workday-benefits-benefit-enrollment-event-offerings-openapi.json
  format: json
  label: Workday Benefit Enrollment Event Offerings API
  slug: workday-benefits-benefit-enrollment-event-offerings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-benefits/refs/heads/main/openapi/workday-benefits-benefit-enrollment-event-offerings-openapi.json
- filename: workday-benefits-benefit-partner-openapi.json
  format: json
  label: Workday Benefit Partner API
  slug: workday-benefits-benefit-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-benefits/refs/heads/main/openapi/workday-benefits-benefit-partner-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: workday.com
  spf: true
hosts:
- cert_expires: Mar 10 23:59:59 2027 GMT
  host: www.workday.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  2 19:44:37 2026 GMT
  host: wd2-impl-services1.workday.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  9 01:18:54 2026 GMT
  host: developer.workday.com
  hsts: true
  hsts_max_age: 15638400
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Workday Benefits Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Workday Benefits, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Workday Benefits
provider_slug: workday-benefits
slug: workday-benefits-domain-security
source_filename: workday-benefits-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.workday.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 10 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: wd2-impl-services1.workday.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 19:44:37 2026 GMT\n  hsts: null\n- host: developer.workday.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 01:18:54 2026 GMT\n  hsts: true\n  hsts_max_age: 15638400\ndomains:\n- domain: workday.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workday-benefits/refs/heads/main/security/workday-benefits-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Benefits
- Human Resources
- HCM
- Enterprise
- Payroll
- Employee Benefits
- SOAP
- OpenAPI
---
