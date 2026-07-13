---
api_specs:
- filename: metals-dev-openapi.yml
  format: yaml
  label: Metals.Dev API
  slug: metals-dev-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metals-dev/refs/heads/main/openapi/metals-dev-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: metals.dev
  spf: false
hosts:
- cert_expires: Sep 19 03:17:14 2026 GMT
  host: metals.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 23:59:20 2026 GMT
  host: api.metals.dev
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Metals Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Metals.Dev, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Metals.Dev
provider_slug: metals-dev
slug: metals-dev-domain-security
source_filename: metals-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: metals.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 03:17:14 2026 GMT\n  hsts: false\n- host: api.metals.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 23:59:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: metals.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/metals-dev/refs/heads/main/security/metals-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Financial Data
- Gold
- Precious Metals
- Silver
- Spot Prices
---
