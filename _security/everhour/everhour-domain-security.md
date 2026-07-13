---
api_specs:
- filename: everhour-openapi.yml
  format: yaml
  label: Everhour Time Records API
  slug: everhour-time-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/everhour/refs/heads/main/openapi/everhour-openapi.yml
- filename: everhour-openapi.yml
  format: yaml
  label: Everhour Timers API
  slug: everhour-timers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/everhour/refs/heads/main/openapi/everhour-openapi.yml
- filename: everhour-openapi.yml
  format: yaml
  label: Everhour Timesheets and Timecards API
  slug: everhour-timesheets-timecards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/everhour/refs/heads/main/openapi/everhour-openapi.yml
- filename: everhour-openapi.yml
  format: yaml
  label: Everhour Projects API
  slug: everhour-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/everhour/refs/heads/main/openapi/everhour-openapi.yml
- filename: everhour-openapi.yml
  format: yaml
  label: Everhour Tasks API
  slug: everhour-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/everhour/refs/heads/main/openapi/everhour-openapi.yml
- filename: everhour-openapi.yml
  format: yaml
  label: Everhour Schedule and Time Off API
  slug: everhour-schedule-time-off-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/everhour/refs/heads/main/openapi/everhour-openapi.yml
- filename: everhour-openapi.yml
  format: yaml
  label: Everhour Clients and Invoices API
  slug: everhour-clients-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/everhour/refs/heads/main/openapi/everhour-openapi.yml
- filename: everhour-openapi.yml
  format: yaml
  label: Everhour Expenses API
  slug: everhour-expenses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/everhour/refs/heads/main/openapi/everhour-openapi.yml
- filename: everhour-openapi.yml
  format: yaml
  label: Everhour Reports API
  slug: everhour-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/everhour/refs/heads/main/openapi/everhour-openapi.yml
- filename: everhour-openapi.yml
  format: yaml
  label: Everhour Users API
  slug: everhour-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/everhour/refs/heads/main/openapi/everhour-openapi.yml
- filename: everhour-openapi.yml
  format: yaml
  label: Everhour Webhooks API
  slug: everhour-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/everhour/refs/heads/main/openapi/everhour-openapi.yml
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
