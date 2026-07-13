---
api_specs:
- filename: timecamp-openapi.yml
  format: yaml
  label: TimeCamp Time Entries API
  slug: timecamp-time-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timecamp/refs/heads/main/openapi/timecamp-openapi.yml
- filename: timecamp-openapi.yml
  format: yaml
  label: TimeCamp Timer API
  slug: timecamp-timer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timecamp/refs/heads/main/openapi/timecamp-openapi.yml
- filename: timecamp-openapi.yml
  format: yaml
  label: TimeCamp Tasks and Projects API
  slug: timecamp-tasks-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timecamp/refs/heads/main/openapi/timecamp-openapi.yml
- filename: timecamp-openapi.yml
  format: yaml
  label: TimeCamp Users and Groups API
  slug: timecamp-users-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timecamp/refs/heads/main/openapi/timecamp-openapi.yml
- filename: timecamp-openapi.yml
  format: yaml
  label: TimeCamp Attendance API
  slug: timecamp-attendance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timecamp/refs/heads/main/openapi/timecamp-openapi.yml
- filename: timecamp-openapi.yml
  format: yaml
  label: TimeCamp Timesheet Approvals API
  slug: timecamp-approvals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timecamp/refs/heads/main/openapi/timecamp-openapi.yml
- filename: timecamp-openapi.yml
  format: yaml
  label: TimeCamp Computer Activities API
  slug: timecamp-computer-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timecamp/refs/heads/main/openapi/timecamp-openapi.yml
- filename: timecamp-openapi.yml
  format: yaml
  label: TimeCamp Tags API
  slug: timecamp-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timecamp/refs/heads/main/openapi/timecamp-openapi.yml
- filename: timecamp-openapi.yml
  format: yaml
  label: TimeCamp Billing Rates and Expenses API
  slug: timecamp-billing-rates-expenses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timecamp/refs/heads/main/openapi/timecamp-openapi.yml
- filename: timecamp-openapi.yml
  format: yaml
  label: TimeCamp Data Export API
  slug: timecamp-data-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timecamp/refs/heads/main/openapi/timecamp-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: timecamp.com
  spf: true
hosts:
- cert_expires: Sep 26 17:47:28 2026 GMT
  host: www.timecamp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 17:47:28 2026 GMT
  host: developer.timecamp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 17:47:28 2026 GMT
  host: app.timecamp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Timecamp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TimeCamp, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: TimeCamp
provider_slug: timecamp
slug: timecamp-domain-security
source_filename: timecamp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.timecamp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 17:47:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.timecamp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 17:47:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.timecamp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 17:47:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: timecamp.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/timecamp/refs/heads/main/security/timecamp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Time Tracking
- Timesheets
- Productivity
- Attendance
- Project Management
- Billing
---
