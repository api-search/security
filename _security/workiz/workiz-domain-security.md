---
api_specs:
- filename: workiz-openapi.yml
  format: yaml
  label: Workiz Jobs API
  slug: workiz-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workiz/refs/heads/main/openapi/workiz-openapi.yml
- filename: workiz-openapi.yml
  format: yaml
  label: Workiz Leads API
  slug: workiz-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workiz/refs/heads/main/openapi/workiz-openapi.yml
- filename: workiz-openapi.yml
  format: yaml
  label: Workiz Team API
  slug: workiz-team-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workiz/refs/heads/main/openapi/workiz-openapi.yml
- filename: workiz-openapi.yml
  format: yaml
  label: Workiz Time Off API
  slug: workiz-time-off-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workiz/refs/heads/main/openapi/workiz-openapi.yml
- filename: workiz-openapi.yml
  format: yaml
  label: Workiz Payments API
  slug: workiz-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workiz/refs/heads/main/openapi/workiz-openapi.yml
- filename: workiz-openapi.yml
  format: yaml
  label: Workiz Webhooks
  slug: workiz-webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workiz/refs/heads/main/openapi/workiz-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: workiz.com
  spf: true
hosts:
- cert_expires: Aug 24 01:42:12 2026 GMT
  host: www.workiz.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 24 23:59:59 2026 GMT
  host: developer.workiz.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 15 06:08:49 2026 GMT
  host: api.workiz.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Workiz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Workiz, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Workiz
provider_slug: workiz
slug: workiz-domain-security
source_filename: workiz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.workiz.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 01:42:12 2026 GMT\n  hsts: false\n- host: developer.workiz.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 23:59:59 2026 GMT\n  hsts: false\n- host: api.workiz.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 06:08:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: workiz.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workiz/refs/heads/main/security/workiz-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Field Service Management
- FSM
- Home Services
- Scheduling
- Dispatch
- CRM
- Jobs
- Invoicing
---
