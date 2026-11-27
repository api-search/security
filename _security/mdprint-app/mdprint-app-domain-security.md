---
api_specs:
- filename: mdprint-app-ask-api-openapi.yml
  format: yaml
  label: mdprint Ask API
  slug: mdprint-app-ask-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mdprint-app/openapi/mdprint-app-ask-api-openapi.yml
- filename: mdprint-app-docs-api-openapi.yml
  format: yaml
  label: mdprint Docs API
  slug: mdprint-app-docs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mdprint-app/openapi/mdprint-app-docs-api-openapi.yml
- filename: mdprint-app-examples-api-openapi.yml
  format: yaml
  label: mdprint Examples API
  slug: mdprint-app-examples-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mdprint-app/openapi/mdprint-app-examples-api-openapi.yml
- filename: mdprint-app-info-api-openapi.yml
  format: yaml
  label: mdprint Info API
  slug: mdprint-app-info-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mdprint-app/openapi/mdprint-app-info-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mdprint.app
  spf: true
hosts:
- cert_expires: Jan 17 09:23:49 2027 GMT
  host: mdprint.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: mdprint Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for mdprint, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: mdprint
provider_slug: mdprint-app
slug: mdprint-app-domain-security
source_filename: mdprint-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mdprint.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 09:23:49 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mdprint.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/mdprint-app/security/mdprint-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Tool
- Markdown
- PDF
- Privacy
- Open Source
---
