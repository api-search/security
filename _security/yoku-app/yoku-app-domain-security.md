---
api_specs:
- filename: yoku-app-openapi-generated.yml
  format: yaml
  label: yoku-app API
  slug: yoku-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/yoku-app/openapi/_ae-authored/yoku-app-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: yoku.app
  spf: true
hosts:
- cert_expires: Dec 15 19:16:39 2026 GMT
  host: yoku.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: yoku-app Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for yoku-app, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: yoku-app
provider_slug: yoku-app
slug: yoku-app-domain-security
source_filename: yoku-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: yoku.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 19:16:39 2026 GMT\n  hsts: false\ndomains:\n- domain: yoku.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/yoku-app/security/yoku-app-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Brands
- Data
- Software-as-a-Service
---
