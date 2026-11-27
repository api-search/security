---
api_specs:
- filename: devmargin-app-openapi-openapi.yml
  format: yaml
  label: DevMargin API Openapi API
  slug: devmargin-api-openapi-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/devmargin-app/openapi/_original/devmargin-app-openapi-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: devmargin.app
  spf: true
hosts:
- cert_expires: Dec 23 09:21:22 2026 GMT
  host: devmargin.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: DevMargin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DevMargin, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: DevMargin
provider_slug: devmargin-app
slug: devmargin-app-domain-security
source_filename: devmargin-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: devmargin.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 09:21:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: devmargin.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/devmargin-app/security/devmargin-app-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
---
