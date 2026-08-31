---
api_specs:
- filename: ritten-calendar-api-openapi.yml
  format: yaml
  label: Ritten Calendar API
  slug: ritten-calendar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ritten/refs/heads/main/openapi/ritten-calendar-api-openapi.yml
- filename: ritten-cases-api-openapi.yml
  format: yaml
  label: Ritten Cases API
  slug: ritten-cases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ritten/refs/heads/main/openapi/ritten-cases-api-openapi.yml
- filename: ritten-contacts-api-openapi.yml
  format: yaml
  label: Ritten Contacts API
  slug: ritten-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ritten/refs/heads/main/openapi/ritten-contacts-api-openapi.yml
- filename: ritten-encounters-api-openapi.yml
  format: yaml
  label: Ritten Encounters API
  slug: ritten-encounters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ritten/refs/heads/main/openapi/ritten-encounters-api-openapi.yml
- filename: ritten-facilities-api-openapi.yml
  format: yaml
  label: Ritten Facilities API
  slug: ritten-facilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ritten/refs/heads/main/openapi/ritten-facilities-api-openapi.yml
- filename: ritten-forms-api-openapi.yml
  format: yaml
  label: Ritten Forms API
  slug: ritten-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ritten/refs/heads/main/openapi/ritten-forms-api-openapi.yml
- filename: ritten-insights-api-openapi.yml
  format: yaml
  label: Ritten Insights API
  slug: ritten-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ritten/refs/heads/main/openapi/ritten-insights-api-openapi.yml
- filename: ritten-insurance-api-openapi.yml
  format: yaml
  label: Ritten Insurance API
  slug: ritten-insurance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ritten/refs/heads/main/openapi/ritten-insurance-api-openapi.yml
- filename: ritten-oauth-api-openapi.yml
  format: yaml
  label: Ritten OAUTH API
  slug: ritten-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ritten/refs/heads/main/openapi/ritten-oauth-api-openapi.yml
- filename: ritten-organizations-api-openapi.yml
  format: yaml
  label: Ritten Organizations API
  slug: ritten-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ritten/refs/heads/main/openapi/ritten-organizations-api-openapi.yml
- filename: ritten-patients-api-openapi.yml
  format: yaml
  label: Ritten Patients API
  slug: ritten-patients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ritten/refs/heads/main/openapi/ritten-patients-api-openapi.yml
- filename: ritten-programs-api-openapi.yml
  format: yaml
  label: Ritten Programs API
  slug: ritten-programs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ritten/refs/heads/main/openapi/ritten-programs-api-openapi.yml
- filename: ritten-tasks-api-openapi.yml
  format: yaml
  label: Ritten Tasks API
  slug: ritten-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ritten/refs/heads/main/openapi/ritten-tasks-api-openapi.yml
- filename: ritten-users-api-openapi.yml
  format: yaml
  label: Ritten Users API
  slug: ritten-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ritten/refs/heads/main/openapi/ritten-users-api-openapi.yml
- filename: ritten-webhooks-api-openapi.yml
  format: yaml
  label: Ritten Webhooks API
  slug: ritten-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ritten/refs/heads/main/openapi/ritten-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: ritten.io
  spf: true
hosts:
- cert_expires: Oct 15 00:40:19 2026 GMT
  host: ritten.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 23:59:59 2026 GMT
  host: api.ritten.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ritten Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ritten, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Ritten
provider_slug: ritten
slug: ritten-domain-security
source_filename: ritten-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ritten.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 00:40:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.ritten.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: ritten.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ritten/refs/heads/main/security/ritten-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Behavioral Health
- EMR
- EHR
- Healthcare
- Practice Management
- HIPAA
- Revenue Cycle Management
- Clinical Documentation
- Telehealth
- OpenAPI
- Webhook
- Behavioral Health API
- Substance Use Treatment
- 42 CFR Part 2
- Electronic Health Records
---
