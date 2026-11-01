---
api_specs:
- filename: maesn-accounting-api-openapi.yml
  format: yaml
  label: Maesn Accounting API
  slug: maesn-accounting-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maesn/openapi/maesn-accounting-api-openapi.yml
- filename: maesn-auth-api-openapi.yml
  format: yaml
  label: Maesn Auth API
  slug: maesn-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maesn/openapi/maesn-auth-api-openapi.yml
- filename: maesn-tenants-api-openapi.yml
  format: yaml
  label: Maesn Tenants API
  slug: maesn-tenants-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maesn/openapi/maesn-tenants-api-openapi.yml
- filename: maesn-user-api-openapi.yml
  format: yaml
  label: Maesn User API
  slug: maesn-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maesn/openapi/maesn-user-api-openapi.yml
- filename: maesn-webhook-api-openapi.yml
  format: yaml
  label: Maesn Webhook API
  slug: maesn-webhook-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maesn/openapi/maesn-webhook-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: maesn.com
  spf: true
hosts:
- cert_expires: Nov 25 13:48:16 2026 GMT
  host: maesn.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Maesn Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Maesn, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Maesn
provider_slug: maesn
slug: maesn-domain-security
source_filename: maesn-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: maesn.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 13:48:16 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: maesn.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/maesn/security/maesn-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- ERP
- Accounting
- Integration
- Software-as-a-Service
---
