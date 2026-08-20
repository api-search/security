---
api_specs:
- filename: zoho-people-attendance-api-openapi.yml
  format: yaml
  label: Zoho People Attendance API
  slug: zoho-people-attendance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoho-people/refs/heads/main/openapi/zoho-people-attendance-api-openapi.yml
- filename: zoho-people-automation-api-openapi.yml
  format: yaml
  label: Zoho People Automation API
  slug: zoho-people-automation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoho-people/refs/heads/main/openapi/zoho-people-automation-api-openapi.yml
- filename: zoho-people-dashboard-api-openapi.yml
  format: yaml
  label: Zoho People Dashboard API
  slug: zoho-people-dashboard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoho-people/refs/heads/main/openapi/zoho-people-dashboard-api-openapi.yml
- filename: zoho-people-employee-api-openapi.yml
  format: yaml
  label: Zoho People Employee API
  slug: zoho-people-employee-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoho-people/refs/heads/main/openapi/zoho-people-employee-api-openapi.yml
- filename: zoho-people-forms-api-openapi.yml
  format: yaml
  label: Zoho People Forms API
  slug: zoho-people-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoho-people/refs/heads/main/openapi/zoho-people-forms-api-openapi.yml
- filename: zoho-people-leave-api-openapi.yml
  format: yaml
  label: Zoho People Leave API
  slug: zoho-people-leave-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoho-people/refs/heads/main/openapi/zoho-people-leave-api-openapi.yml
- filename: zoho-people-time-tracker-api-openapi.yml
  format: yaml
  label: Zoho People Time Tracker API
  slug: zoho-people-time-tracker-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoho-people/refs/heads/main/openapi/zoho-people-time-tracker-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zoho.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zoho.eu
  spf: true
hosts:
- cert_expires: Sep 26 23:59:59 2026 GMT
  host: www.zoho.com
  hsts: true
  hsts_max_age: 64072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 22 23:59:59 2026 GMT
  host: people.zoho.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 25 23:59:59 2026 GMT
  host: people.zoho.eu
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zoho People Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zoho People, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Zoho People
provider_slug: zoho-people
slug: zoho-people-domain-security
source_filename: zoho-people-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zoho.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 64072000\n- host: people.zoho.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 23:59:59 2026 GMT\n  hsts: null\n- host: people.zoho.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: zoho.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: zoho.eu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zoho-people/refs/heads/main/security/zoho-people-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- HR
- HRMS
- Human Resources
- HRIS
- Employee Management
- Attendance
- Leave Management
- Time Tracking
- Performance Management
- Onboarding
- Zoho
- Authentication
---
