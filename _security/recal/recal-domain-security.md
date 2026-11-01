---
api_specs:
- filename: recal-organization-api-openapi.yml
  format: yaml
  label: Recal Organization API
  slug: recal-organization-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/recal/openapi/recal-organization-api-openapi.yml
- filename: recal-organization-scheduling-api-openapi.yml
  format: yaml
  label: Recal Organization Scheduling API
  slug: recal-organization-scheduling-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/recal/openapi/recal-organization-scheduling-api-openapi.yml
- filename: recal-organizations-calendar-api-openapi.yml
  format: yaml
  label: Recal Organizations Calendar API
  slug: recal-organizations-calendar-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/recal/openapi/recal-organizations-calendar-api-openapi.yml
- filename: recal-user-calendar-api-openapi.yml
  format: yaml
  label: Recal User Calendar API
  slug: recal-user-calendar-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/recal/openapi/recal-user-calendar-api-openapi.yml
- filename: recal-user-oauth-api-openapi.yml
  format: yaml
  label: Recal User OAuth API
  slug: recal-user-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/recal/openapi/recal-user-oauth-api-openapi.yml
- filename: recal-user-scheduling-api-openapi.yml
  format: yaml
  label: Recal User Scheduling API
  slug: recal-user-scheduling-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/recal/openapi/recal-user-scheduling-api-openapi.yml
- filename: recal-users-api-openapi.yml
  format: yaml
  label: Recal Users API
  slug: recal-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/recal/openapi/recal-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: recal.dev
  spf: false
hosts:
- cert_expires: Dec 12 00:39:22 2026 GMT
  host: recal.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Recal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Recal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Recal
provider_slug: recal
slug: recal-domain-security
source_filename: recal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: recal.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 00:39:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: recal.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/recal/security/recal-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Calendar API
- Scheduling
- SDK
- Multi-Tenant
- Recruiting
- Marketplace
- AI Agents
---
