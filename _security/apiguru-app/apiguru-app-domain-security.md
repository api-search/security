---
api_specs:
- filename: apiguru-app-amazon-data-api-openapi.yml
  format: yaml
  label: apiguru-app Amazon Data API
  slug: apiguru-app-amazon-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apiguru-app/openapi/apiguru-app-amazon-data-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: apiguru.app
  spf: true
hosts:
- cert_expires: Dec 25 07:21:14 2026 GMT
  host: apiguru.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Apiguru App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for apiguru-app, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: apiguru-app
provider_slug: apiguru-app
slug: apiguru-app-domain-security
source_filename: apiguru-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apiguru.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 07:21:14 2026 GMT\n  hsts: false\ndomains:\n- domain: apiguru.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/apiguru-app/security/apiguru-app-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- API
- Data
- Amazon
- Real-time
- Integration
---
