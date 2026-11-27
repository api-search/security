---
api_specs:
- filename: compatlab-me-packages-api-openapi.yml
  format: yaml
  label: CompatLab Packages API
  slug: compatlab-me-packages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compatlab-me/openapi/compatlab-me-packages-api-openapi.yml
- filename: compatlab-me-reports-api-openapi.yml
  format: yaml
  label: CompatLab Reports API
  slug: compatlab-me-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compatlab-me/openapi/compatlab-me-reports-api-openapi.yml
- filename: compatlab-me-scans-api-openapi.yml
  format: yaml
  label: CompatLab Scans API
  slug: compatlab-me-scans-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compatlab-me/openapi/compatlab-me-scans-api-openapi.yml
- filename: compatlab-me-search-api-openapi.yml
  format: yaml
  label: CompatLab Search API
  slug: compatlab-me-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compatlab-me/openapi/compatlab-me-search-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: compatlab.me
  spf: false
hosts:
- cert_expires: Jan  2 14:19:21 2027 GMT
  host: compatlab.me
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: CompatLab Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CompatLab, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: CompatLab
provider_slug: compatlab-me
slug: compatlab-me-domain-security
source_filename: compatlab-me-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: compatlab.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 14:19:21 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: compatlab.me\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/compatlab-me/security/compatlab-me-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- npm
- JavaScript
- Node.js
- Bun
- Deno
- Compatibility Testing
- Developer Tools
- Open Source
- MCP
---
