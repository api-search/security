---
api_specs:
- filename: hubstaff-openapi.yml
  format: yaml
  label: Hubstaff Activities and Time Tracking API
  slug: hubstaff-activities-time-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hubstaff/refs/heads/main/openapi/hubstaff-openapi.yml
- filename: hubstaff-openapi.yml
  format: yaml
  label: Hubstaff Timesheets and Time Entries API
  slug: hubstaff-timesheets-time-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hubstaff/refs/heads/main/openapi/hubstaff-openapi.yml
- filename: hubstaff-openapi.yml
  format: yaml
  label: Hubstaff Organizations and Teams API
  slug: hubstaff-organizations-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hubstaff/refs/heads/main/openapi/hubstaff-openapi.yml
- filename: hubstaff-openapi.yml
  format: yaml
  label: Hubstaff Projects and Tasks API
  slug: hubstaff-projects-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hubstaff/refs/heads/main/openapi/hubstaff-openapi.yml
- filename: hubstaff-openapi.yml
  format: yaml
  label: Hubstaff Users API
  slug: hubstaff-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hubstaff/refs/heads/main/openapi/hubstaff-openapi.yml
- filename: hubstaff-openapi.yml
  format: yaml
  label: Hubstaff Time Off and Attendance API
  slug: hubstaff-time-off-attendance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hubstaff/refs/heads/main/openapi/hubstaff-openapi.yml
- filename: hubstaff-openapi.yml
  format: yaml
  label: Hubstaff Clients, Invoices, and Payments API
  slug: hubstaff-clients-invoices-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hubstaff/refs/heads/main/openapi/hubstaff-openapi.yml
- filename: hubstaff-openapi.yml
  format: yaml
  label: Hubstaff Screenshots and App Tracking API
  slug: hubstaff-screenshots-app-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hubstaff/refs/heads/main/openapi/hubstaff-openapi.yml
- filename: hubstaff-openapi.yml
  format: yaml
  label: Hubstaff Webhooks API
  slug: hubstaff-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hubstaff/refs/heads/main/openapi/hubstaff-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:dev-sec-ops@hubstaff.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: hubstaff.com
  spf: true
hosts:
- cert_expires: Nov  4 11:07:13 2026 GMT
  host: hubstaff.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  4 11:07:13 2026 GMT
  host: developer.hubstaff.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  4 11:07:13 2026 GMT
  host: api.hubstaff.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hubstaff Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hubstaff, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Hubstaff
provider_slug: hubstaff
slug: hubstaff-domain-security
source_filename: hubstaff-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hubstaff.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 11:07:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.hubstaff.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 11:07:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.hubstaff.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 11:07:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hubstaff.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:dev-sec-ops@hubstaff.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hubstaff/refs/heads/main/security/hubstaff-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Time Tracking
- Timesheets
- Workforce Management
- Productivity
- Employee Monitoring
- Project Management
- Payroll
---
