---
api_specs:
- filename: workday-report-writer-raas-openapi.yml
  format: yaml
  label: Workday Report-as-a-Service (RaaS) REST API
  slug: workday-report-as-a-service-raas-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-report-writer/refs/heads/main/openapi/workday-report-writer-raas-openapi.yml
- filename: workday-report-writer-wql-openapi.yml
  format: yaml
  label: Workday WQL API
  slug: workday-wql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-report-writer/refs/heads/main/openapi/workday-report-writer-wql-openapi.yml
- filename: workday-report-writer-prism-analytics-openapi.yml
  format: yaml
  label: Workday Prism Analytics API
  slug: workday-prism-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-report-writer/refs/heads/main/openapi/workday-report-writer-prism-analytics-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: workday.com
  spf: true
hosts:
- cert_expires: Aug 21 03:09:01 2026 GMT
  host: developer.workday.com
  hsts: true
  hsts_max_age: 15638400
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: www.workday.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 03:30:49 2026 GMT
  host: wd2-impl-services1.workday.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Workday Report Writer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Workday Report Writer, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Workday Report Writer
provider_slug: workday-report-writer
slug: workday-report-writer-domain-security
source_filename: workday-report-writer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.workday.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 03:09:01 2026 GMT\n  hsts: true\n  hsts_max_age: 15638400\n- host: www.workday.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: wd2-impl-services1.workday.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 03:30:49 2026 GMT\n  hsts: null\ndomains:\n- domain: workday.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workday-report-writer/refs/heads/main/security/workday-report-writer-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- Enterprise
- Erp
- Financials
- Hrms
- Reporting
- Saas
---
