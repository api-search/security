---
api_specs:
- filename: tamloot-cc-account-api-openapi.yml
  format: yaml
  label: Tamloot Account API
  slug: tamloot-cc-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tamloot-cc/openapi/tamloot-cc-account-api-openapi.yml
- filename: tamloot-cc-changes-api-openapi.yml
  format: yaml
  label: Tamloot Changes API
  slug: tamloot-cc-changes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tamloot-cc/openapi/tamloot-cc-changes-api-openapi.yml
- filename: tamloot-cc-contacts-api-openapi.yml
  format: yaml
  label: Tamloot Contacts API
  slug: tamloot-cc-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tamloot-cc/openapi/tamloot-cc-contacts-api-openapi.yml
- filename: tamloot-cc-health-api-openapi.yml
  format: yaml
  label: Tamloot Health API
  slug: tamloot-cc-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tamloot-cc/openapi/tamloot-cc-health-api-openapi.yml
- filename: tamloot-cc-me-api-openapi.yml
  format: yaml
  label: Tamloot Me API
  slug: tamloot-cc-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tamloot-cc/openapi/tamloot-cc-me-api-openapi.yml
- filename: tamloot-cc-notes-api-openapi.yml
  format: yaml
  label: Tamloot Notes API
  slug: tamloot-cc-notes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tamloot-cc/openapi/tamloot-cc-notes-api-openapi.yml
- filename: tamloot-cc-read-api-api-openapi.yml
  format: yaml
  label: Tamloot Read API
  slug: tamloot-cc-read-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tamloot-cc/openapi/tamloot-cc-read-api-api-openapi.yml
- filename: tamloot-cc-service-api-openapi.yml
  format: yaml
  label: Tamloot Service API
  slug: tamloot-cc-service-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tamloot-cc/openapi/tamloot-cc-service-api-openapi.yml
- filename: tamloot-cc-sessions-api-openapi.yml
  format: yaml
  label: Tamloot Sessions API
  slug: tamloot-cc-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tamloot-cc/openapi/tamloot-cc-sessions-api-openapi.yml
- filename: tamloot-cc-tasks-api-openapi.yml
  format: yaml
  label: Tamloot Tasks API
  slug: tamloot-cc-tasks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tamloot-cc/openapi/tamloot-cc-tasks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dns_aid:
    checked: '2026-11-26'
    published: false
  dnssec: false
  domain: tamloot.cc
  spf: true
hosts:
- cert_expires: Jan 11 03:20:49 2027 GMT
  host: tamloot.cc
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Tamloot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tamloot, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Tamloot
provider_slug: tamloot-cc
slug: tamloot-cc-domain-security
source_filename: tamloot-cc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tamloot.cc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 03:20:49 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: tamloot.cc\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n  dns_aid:\n    checked: '2026-11-26'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/tamloot-cc/security/tamloot-cc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- CRM
- Business
- Productivity
- Small Business
---
