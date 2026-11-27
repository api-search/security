---
api_specs:
- filename: dilutionlens-com-company-api-openapi.yml
  format: yaml
  label: DilutionLens Company API
  slug: dilutionlens-com-company-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dilutionlens-com/openapi/dilutionlens-com-company-api-openapi.yml
- filename: dilutionlens-com-screen-api-openapi.yml
  format: yaml
  label: DilutionLens Screen API
  slug: dilutionlens-com-screen-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dilutionlens-com/openapi/dilutionlens-com-screen-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dilutionlens.com
  spf: true
hosts:
- cert_expires: Feb 11 23:59:59 2027 GMT
  host: dilutionlens.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: DilutionLens Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DilutionLens, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: DilutionLens
provider_slug: dilutionlens-com
slug: dilutionlens-com-domain-security
source_filename: dilutionlens-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dilutionlens.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 11 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dilutionlens.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/dilutionlens-com/security/dilutionlens-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Financial Data
- Capital Markets
- ASX
- Equity Dilution
- Market Data
- MCP
- Investing
---
