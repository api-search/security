---
api_specs:
- filename: everhour-clients-api-openapi.yml
  format: yaml
  label: Everhour Clients API
  slug: everhour-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/everhour/refs/heads/main/openapi/everhour-clients-api-openapi.yml
- filename: everhour-expenses-api-openapi.yml
  format: yaml
  label: Everhour Expenses API
  slug: everhour-expenses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/everhour/refs/heads/main/openapi/everhour-expenses-api-openapi.yml
- filename: everhour-invoices-api-openapi.yml
  format: yaml
  label: Everhour Invoices API
  slug: everhour-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/everhour/refs/heads/main/openapi/everhour-invoices-api-openapi.yml
- filename: everhour-projects-api-openapi.yml
  format: yaml
  label: Everhour Projects API
  slug: everhour-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/everhour/refs/heads/main/openapi/everhour-projects-api-openapi.yml
- filename: everhour-reports-api-openapi.yml
  format: yaml
  label: Everhour Reports API
  slug: everhour-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/everhour/refs/heads/main/openapi/everhour-reports-api-openapi.yml
- filename: everhour-schedule-api-openapi.yml
  format: yaml
  label: Everhour Schedule API
  slug: everhour-schedule-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/everhour/refs/heads/main/openapi/everhour-schedule-api-openapi.yml
- filename: everhour-tasks-api-openapi.yml
  format: yaml
  label: Everhour Tasks API
  slug: everhour-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/everhour/refs/heads/main/openapi/everhour-tasks-api-openapi.yml
- filename: everhour-time-off-api-openapi.yml
  format: yaml
  label: Everhour Time Off API
  slug: everhour-time-off-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/everhour/refs/heads/main/openapi/everhour-time-off-api-openapi.yml
- filename: everhour-time-records-api-openapi.yml
  format: yaml
  label: Everhour Time Records API
  slug: everhour-time-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/everhour/refs/heads/main/openapi/everhour-time-records-api-openapi.yml
- filename: everhour-timecards-api-openapi.yml
  format: yaml
  label: Everhour Timecards API
  slug: everhour-timecards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/everhour/refs/heads/main/openapi/everhour-timecards-api-openapi.yml
- filename: everhour-timers-api-openapi.yml
  format: yaml
  label: Everhour Timers API
  slug: everhour-timers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/everhour/refs/heads/main/openapi/everhour-timers-api-openapi.yml
- filename: everhour-timesheets-api-openapi.yml
  format: yaml
  label: Everhour Timesheets API
  slug: everhour-timesheets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/everhour/refs/heads/main/openapi/everhour-timesheets-api-openapi.yml
- filename: everhour-users-api-openapi.yml
  format: yaml
  label: Everhour Users API
  slug: everhour-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/everhour/refs/heads/main/openapi/everhour-users-api-openapi.yml
- filename: everhour-webhooks-api-openapi.yml
  format: yaml
  label: Everhour Webhooks API
  slug: everhour-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/everhour/refs/heads/main/openapi/everhour-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: everhour.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: apiary.io
  spf: true
hosts:
- cert_expires: Dec 27 08:44:24 2026 GMT
  host: everhour.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 18 23:59:59 2026 GMT
  host: everhour.docs.apiary.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 27 08:44:24 2026 GMT
  host: api.everhour.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Everhour Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Everhour, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Everhour
provider_slug: everhour
slug: everhour-domain-security
source_filename: everhour-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: everhour.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 08:44:24 2026 GMT\n  hsts: false\n- host: everhour.docs.apiary.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 23:59:59 2026 GMT\n  hsts: null\n- host: api.everhour.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 27 08:44:24 2026 GMT\n  hsts: false\ndomains:\n- domain: everhour.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: apiary.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/everhour/refs/heads/main/security/everhour-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Time Tracking
- Timesheets
- Productivity
- Project Management
- Budgeting
- Invoicing
---
