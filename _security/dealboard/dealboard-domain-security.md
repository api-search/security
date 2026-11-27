---
api_specs:
- filename: dealboard-deals-api-openapi.yml
  format: yaml
  label: Dealboard Deals API
  slug: dealboard-deals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dealboard/openapi/dealboard-deals-api-openapi.yml
- filename: dealboard-reports-api-openapi.yml
  format: yaml
  label: Dealboard Reports API
  slug: dealboard-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dealboard/openapi/dealboard-reports-api-openapi.yml
- filename: dealboard-templates-api-openapi.yml
  format: yaml
  label: Dealboard Templates API
  slug: dealboard-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dealboard/openapi/dealboard-templates-api-openapi.yml
- filename: dealboard-auth-api-openapi.yml
  format: yaml
  label: Dealboard Auth API
  slug: dealboard-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dealboard/openapi/dealboard-auth-api-openapi.yml
- filename: dealboard-boards-api-openapi.yml
  format: yaml
  label: Dealboard Boards API
  slug: dealboard-boards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dealboard/openapi/dealboard-boards-api-openapi.yml
- filename: dealboard-dealboard-api-api-openapi.yml
  format: yaml
  label: Dealboard Dealboard API
  slug: dealboard-dealboard-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dealboard/openapi/dealboard-dealboard-api-api-openapi.yml
- filename: dealboard-leads-api-openapi.yml
  format: yaml
  label: Dealboard Leads API
  slug: dealboard-leads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dealboard/openapi/dealboard-leads-api-openapi.yml
- filename: dealboard-match-api-openapi.yml
  format: yaml
  label: Dealboard Match API
  slug: dealboard-match-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dealboard/openapi/dealboard-match-api-openapi.yml
- filename: dealboard-notes-api-openapi.yml
  format: yaml
  label: Dealboard Notes API
  slug: dealboard-notes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dealboard/openapi/dealboard-notes-api-openapi.yml
- filename: dealboard-webhooks-api-openapi.yml
  format: yaml
  label: Dealboard Webhooks API
  slug: dealboard-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dealboard/openapi/dealboard-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: getdealboard.com
  spf: true
hosts:
- cert_expires: Feb  6 07:46:20 2027 GMT
  host: getdealboard.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 12 11:50:46 2026 GMT
  host: app.getdealboard.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Dealboard Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dealboard, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Dealboard
provider_slug: dealboard
slug: dealboard-domain-security
source_filename: dealboard-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getdealboard.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  6 07:46:20 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: app.getdealboard.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 11:50:46 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: getdealboard.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/dealboard/security/dealboard-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- CRM
- Sales
- Artificial Intelligence
- Integration
---
