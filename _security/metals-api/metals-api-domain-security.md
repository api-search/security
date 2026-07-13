---
api_specs:
- filename: metals-api-openapi.yml
  format: yaml
  label: Metals-API
  slug: metals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metals-api/refs/heads/main/openapi/metals-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: metals-api.com
  spf: true
hosts:
- cert_expires: Sep 18 02:43:54 2026 GMT
  host: metals-api.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Metals Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Metals-API, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Metals-API
provider_slug: metals-api
slug: metals-api-domain-security
source_filename: metals-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: metals-api.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 02:43:54 2026 GMT\n  hsts: false\ndomains:\n- domain: metals-api.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/metals-api/refs/heads/main/security/metals-api-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Currency
- Financial Data
- Gold
- Precious Metals
- Silver
---
