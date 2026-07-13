---
api_specs:
- filename: hcm.yml
  format: yaml
  label: Workday HCM API
  slug: hcm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/openapi/hcm.yml
- filename: financialManagement.yml
  format: yaml
  label: Workday Financial Management API
  slug: financial-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/openapi/financialManagement.yml
- filename: recruiting.yml
  format: yaml
  label: Workday Recruiting API
  slug: recruiting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/openapi/recruiting.yml
- filename: timeTracking.yml
  format: yaml
  label: Workday Time Tracking API
  slug: time-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/openapi/timeTracking.yml
- filename: benefits.yml
  format: yaml
  label: Workday Benefits API
  slug: benefits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/openapi/benefits.yml
- filename: absenceManagement.yml
  format: yaml
  label: Workday Absence Management API
  slug: absence-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/openapi/absenceManagement.yml
- filename: compensation.yml
  format: yaml
  label: Workday Compensation API
  slug: compensation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/openapi/compensation.yml
- filename: payroll.yml
  format: yaml
  label: Workday Payroll API
  slug: payroll-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/openapi/payroll.yml
- filename: person.yml
  format: yaml
  label: Workday Person API
  slug: person-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/openapi/person.yml
- filename: performanceManagement.yml
  format: yaml
  label: Workday Performance Management API
  slug: performance-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/openapi/performanceManagement.yml
- filename: talent.yml
  format: yaml
  label: Workday Talent Management API
  slug: talent-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/openapi/talent.yml
- filename: common.yml
  format: yaml
  label: Workday Common API
  slug: common-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/openapi/common.yml
- filename: staffing.yml
  format: yaml
  label: Workday Staffing API
  slug: staffing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/openapi/staffing.yml
- filename: prismAnalytics.yml
  format: yaml
  label: Workday Prism Analytics API
  slug: prism-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/openapi/prismAnalytics.yml
- filename: raas.yml
  format: yaml
  label: Workday Report-as-a-Service API
  slug: raas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/openapi/raas.yml
- filename: wql.yml
  format: yaml
  label: Workday WQL API
  slug: wql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/openapi/wql.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: workday.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: workdayspend.com
  spf: false
hosts:
- cert_expires: Sep 10 23:59:59 2026 GMT
  host: community.workday.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 03:30:49 2026 GMT
  host: wd2-impl-services1.workday.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 16 23:59:59 2026 GMT
  host: apidocs.workdayspend.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Workday Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Workday, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Workday
provider_slug: workday
slug: workday-domain-security
source_filename: workday-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: community.workday.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 23:59:59 2026 GMT\n  hsts: null\n- host: wd2-impl-services1.workday.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 03:30:49 2026 GMT\n  hsts: null\n- host: apidocs.workdayspend.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 16 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: workday.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: workdayspend.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/security/workday-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Cloud Computing
- Enterprise Software
- Financial Management
- HCM
- SaaS
---
