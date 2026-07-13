---
api_specs:
- filename: carapi-openapi.yml
  format: yaml
  label: CarAPI
  slug: carapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carapi/refs/heads/main/openapi/carapi-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: carapi.app
  spf: true
hosts:
- cert_expires: Oct  4 11:14:32 2026 GMT
  host: carapi.app
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Carapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CarAPI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: CarAPI
provider_slug: carapi
slug: carapi-domain-security
source_filename: carapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: carapi.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 11:14:32 2026 GMT\n  hsts: false\ndomains:\n- domain: carapi.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carapi/refs/heads/main/security/carapi-domain-security.yml
summary_line: TLSv1.3
tags:
- Automobiles
- Vehicles
---
