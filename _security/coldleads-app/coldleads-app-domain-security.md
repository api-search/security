---
api_specs:
- filename: coldleads-app-activity-api-openapi.yml
  format: yaml
  label: Cold Leads Activity API
  slug: coldleads-app-activity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coldleads-app/openapi/coldleads-app-activity-api-openapi.yml
- filename: coldleads-app-credits-api-openapi.yml
  format: yaml
  label: Cold Leads Credits API
  slug: coldleads-app-credits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coldleads-app/openapi/coldleads-app-credits-api-openapi.yml
- filename: coldleads-app-find-api-openapi.yml
  format: yaml
  label: Cold Leads Find API
  slug: coldleads-app-find-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coldleads-app/openapi/coldleads-app-find-api-openapi.yml
- filename: coldleads-app-follow-ups-api-openapi.yml
  format: yaml
  label: Cold Leads Follow Ups API
  slug: coldleads-app-follow-ups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coldleads-app/openapi/coldleads-app-follow-ups-api-openapi.yml
- filename: coldleads-app-leads-api-openapi.yml
  format: yaml
  label: Cold Leads Leads API
  slug: coldleads-app-leads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coldleads-app/openapi/coldleads-app-leads-api-openapi.yml
- filename: coldleads-app-next-actions-api-openapi.yml
  format: yaml
  label: Cold Leads Next Actions API
  slug: coldleads-app-next-actions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coldleads-app/openapi/coldleads-app-next-actions-api-openapi.yml
- filename: coldleads-app-social-api-openapi.yml
  format: yaml
  label: Cold Leads Social API
  slug: coldleads-app-social-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coldleads-app/openapi/coldleads-app-social-api-openapi.yml
- filename: coldleads-app-verify-api-openapi.yml
  format: yaml
  label: Cold Leads Verify API
  slug: coldleads-app-verify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coldleads-app/openapi/coldleads-app-verify-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: coldleads.app
  spf: true
hosts:
- cert_expires: Jan 27 18:45:58 2027 GMT
  host: coldleads.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Coldleads App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cold Leads, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cold Leads
provider_slug: coldleads-app
slug: coldleads-app-domain-security
source_filename: coldleads-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: coldleads.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 18:45:58 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: coldleads.app\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/coldleads-app/security/coldleads-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CRM
- Software-as-a-Service
- Small Business
- Lead Management
- Cold Leads
---
