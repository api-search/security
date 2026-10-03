---
api_specs:
- filename: sahifa-convert-api-openapi.yml
  format: yaml
  label: Sahifa Convert API
  slug: sahifa-convert-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sahifa/refs/heads/main/openapi/sahifa-convert-api-openapi.yml
- filename: sahifa-health-api-openapi.yml
  format: yaml
  label: Sahifa Health API
  slug: sahifa-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sahifa/refs/heads/main/openapi/sahifa-health-api-openapi.yml
- filename: sahifa-take-api-openapi.yml
  format: yaml
  label: Sahifa Take API
  slug: sahifa-take-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sahifa/refs/heads/main/openapi/sahifa-take-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sahifa.dev
  spf: true
hosts:
- cert_expires: Dec 23 11:35:48 2026 GMT
  host: sahifa.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 23 11:35:49 2026 GMT
  host: api.sahifa.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Sahifa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sahifa, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Sahifa
provider_slug: sahifa
slug: sahifa-domain-security
source_filename: sahifa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sahifa.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 11:35:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.sahifa.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 11:35:49 2026 GMT\n  hsts: null\ndomains:\n- domain: sahifa.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sahifa/refs/heads/main/security/sahifa-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- PDF
- Screenshots
- Saudi Arabia
- Cloud
---
