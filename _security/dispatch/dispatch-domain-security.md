---
api_specs:
- filename: dispatch-appointments-api-openapi.yml
  format: yaml
  label: Dispatch Appointments API
  slug: dispatch-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dispatch/refs/heads/main/openapi/dispatch-appointments-api-openapi.yml
- filename: dispatch-authentication-api-openapi.yml
  format: yaml
  label: Dispatch Authentication API
  slug: dispatch-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dispatch/refs/heads/main/openapi/dispatch-authentication-api-openapi.yml
- filename: dispatch-brands-api-openapi.yml
  format: yaml
  label: Dispatch Brands API
  slug: dispatch-brands-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dispatch/refs/heads/main/openapi/dispatch-brands-api-openapi.yml
- filename: dispatch-customers-api-openapi.yml
  format: yaml
  label: Dispatch Customers API
  slug: dispatch-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dispatch/refs/heads/main/openapi/dispatch-customers-api-openapi.yml
- filename: dispatch-files-api-openapi.yml
  format: yaml
  label: Dispatch Files API
  slug: dispatch-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dispatch/refs/heads/main/openapi/dispatch-files-api-openapi.yml
- filename: dispatch-jobs-api-openapi.yml
  format: yaml
  label: Dispatch Jobs API
  slug: dispatch-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dispatch/refs/heads/main/openapi/dispatch-jobs-api-openapi.yml
- filename: dispatch-organizations-api-openapi.yml
  format: yaml
  label: Dispatch Organizations API
  slug: dispatch-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dispatch/refs/heads/main/openapi/dispatch-organizations-api-openapi.yml
- filename: dispatch-sources-api-openapi.yml
  format: yaml
  label: Dispatch Sources API
  slug: dispatch-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dispatch/refs/heads/main/openapi/dispatch-sources-api-openapi.yml
- filename: dispatch-survey-responses-api-openapi.yml
  format: yaml
  label: Dispatch Survey Responses API
  slug: dispatch-survey-responses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dispatch/refs/heads/main/openapi/dispatch-survey-responses-api-openapi.yml
- filename: dispatch-users-api-openapi.yml
  format: yaml
  label: Dispatch Users API
  slug: dispatch-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dispatch/refs/heads/main/openapi/dispatch-users-api-openapi.yml
- filename: dispatch-work-orders-api-openapi.yml
  format: yaml
  label: Dispatch Work Orders API
  slug: dispatch-work-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dispatch/refs/heads/main/openapi/dispatch-work-orders-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dispatch.me
  spf: true
hosts:
- cert_expires: Oct  2 17:28:00 2026 GMT
  host: dispatch.me
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 22 23:59:59 2026 GMT
  host: api.dispatch.me
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 22 23:59:59 2026 GMT
  host: files-api.dispatch.me
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Dispatch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dispatch, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Dispatch
provider_slug: dispatch
slug: dispatch-domain-security
source_filename: dispatch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dispatch.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 17:28:00 2026 GMT\n  hsts: false\n- host: api.dispatch.me\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: files-api.dispatch.me\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 22 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: dispatch.me\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dispatch/refs/heads/main/security/dispatch-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Field Service
- Service Orchestration
- Work Orders
- Scheduling
- Contractor Networks
- Home Services
- Warranty
- Customer Experience
- Logistics
- Company
---
