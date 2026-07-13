---
api_specs:
- filename: workday-tracking-system-time-tracking-openapi.yml
  format: yaml
  label: Workday Time Tracking API
  slug: workday-time-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-tracking-system/refs/heads/main/openapi/workday-tracking-system-time-tracking-openapi.yml
- filename: workday-tracking-system-absence-management-openapi.yml
  format: yaml
  label: Workday Absence Management API
  slug: workday-absence-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-tracking-system/refs/heads/main/openapi/workday-tracking-system-absence-management-openapi.yml
- filename: workday-tracking-system-scheduling-openapi.yml
  format: yaml
  label: Workday Scheduling API
  slug: workday-scheduling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-tracking-system/refs/heads/main/openapi/workday-tracking-system-scheduling-openapi.yml
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
kind: domain-security
layout: security
method: probed
name: Workday Tracking System Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Workday Tracking System, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Workday Tracking System
provider_slug: workday-tracking-system
slug: workday-tracking-system-domain-security
source_filename: workday-tracking-system-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.workday.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 03:09:01 2026 GMT\n  hsts: true\n  hsts_max_age: 15638400\n- host: www.workday.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: workday.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workday-tracking-system/refs/heads/main/security/workday-tracking-system-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Absence Management
- Attendance
- Enterprise
- HCM
- Human Capital Management
- Payroll
- Scheduling
- Time Tracking
- Timesheets
- Workforce Management
---
