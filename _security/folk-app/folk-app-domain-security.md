---
api_specs:
- filename: folk-app-openapi.yml
  format: yaml
  label: Folk People API
  slug: folk-app-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/folk-app/refs/heads/main/openapi/folk-app-openapi.yml
- filename: folk-app-openapi.yml
  format: yaml
  label: Folk Companies API
  slug: folk-app-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/folk-app/refs/heads/main/openapi/folk-app-openapi.yml
- filename: folk-app-openapi.yml
  format: yaml
  label: Folk Deals and Custom Objects API
  slug: folk-app-deals-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/folk-app/refs/heads/main/openapi/folk-app-openapi.yml
- filename: folk-app-openapi.yml
  format: yaml
  label: Folk Groups API
  slug: folk-app-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/folk-app/refs/heads/main/openapi/folk-app-openapi.yml
- filename: folk-app-openapi.yml
  format: yaml
  label: Folk Notes API
  slug: folk-app-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/folk-app/refs/heads/main/openapi/folk-app-openapi.yml
- filename: folk-app-openapi.yml
  format: yaml
  label: Folk Reminders API
  slug: folk-app-reminders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/folk-app/refs/heads/main/openapi/folk-app-openapi.yml
- filename: folk-app-openapi.yml
  format: yaml
  label: Folk Interactions API
  slug: folk-app-interactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/folk-app/refs/heads/main/openapi/folk-app-openapi.yml
- filename: folk-app-openapi.yml
  format: yaml
  label: Folk Users API
  slug: folk-app-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/folk-app/refs/heads/main/openapi/folk-app-openapi.yml
- filename: folk-app-openapi.yml
  format: yaml
  label: Folk Webhooks API
  slug: folk-app-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/folk-app/refs/heads/main/openapi/folk-app-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: folk.app
  spf: true
hosts:
- cert_expires: Aug 16 14:59:43 2026 GMT
  host: www.folk.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 06:35:33 2026 GMT
  host: developer.folk.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 22 23:59:59 2027 GMT
  host: api.folk.app
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Folk App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Folk, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Folk
provider_slug: folk-app
slug: folk-app-domain-security
source_filename: folk-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.folk.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 14:59:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.folk.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 06:35:33 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.folk.app\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 22 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: folk.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/folk-app/refs/heads/main/security/folk-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CRM
- Relationships
- Contacts
- Sales
- Pipeline
- Webhooks
---
