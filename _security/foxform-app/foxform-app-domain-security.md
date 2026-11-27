---
api_specs:
- filename: foxform-app-analytics-api-openapi.yml
  format: yaml
  label: FoxForm Analytics API
  slug: foxform-app-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/foxform-app/openapi/foxform-app-analytics-api-openapi.yml
- filename: foxform-app-forms-api-openapi.yml
  format: yaml
  label: FoxForm Forms API
  slug: foxform-app-forms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/foxform-app/openapi/foxform-app-forms-api-openapi.yml
- filename: foxform-app-integrations-api-openapi.yml
  format: yaml
  label: FoxForm Integrations API
  slug: foxform-app-integrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/foxform-app/openapi/foxform-app-integrations-api-openapi.yml
- filename: foxform-app-responses-api-openapi.yml
  format: yaml
  label: FoxForm Responses API
  slug: foxform-app-responses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/foxform-app/openapi/foxform-app-responses-api-openapi.yml
- filename: foxform-app-users-api-openapi.yml
  format: yaml
  label: FoxForm Users API
  slug: foxform-app-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/foxform-app/openapi/foxform-app-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: foxform.app
  spf: true
hosts:
- cert_expires: Mar  8 23:59:59 2027 GMT
  host: foxform.app
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: FoxForm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FoxForm, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: FoxForm
provider_slug: foxform-app
slug: foxform-app-domain-security
source_filename: foxform-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: foxform.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  8 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 86400\ndomains:\n- domain: foxform.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/foxform-app/security/foxform-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Form Builder
- Surveys
- Quiz
- Artificial Intelligence
---
