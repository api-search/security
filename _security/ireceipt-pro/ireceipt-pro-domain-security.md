---
api_specs:
- filename: ireceipt-pro-jpg-api-openapi.yml
  format: yaml
  label: ireceipt-pro /jpg API
  slug: ireceipt-pro-jpg-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ireceipt-pro/openapi/ireceipt-pro-jpg-api-openapi.yml
- filename: ireceipt-pro-pdf-api-openapi.yml
  format: yaml
  label: ireceipt-pro /pdf API
  slug: ireceipt-pro-pdf-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ireceipt-pro/openapi/ireceipt-pro-pdf-api-openapi.yml
- filename: ireceipt-pro-ping-api-openapi.yml
  format: yaml
  label: ireceipt-pro /ping API
  slug: ireceipt-pro-ping-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ireceipt-pro/openapi/ireceipt-pro-ping-api-openapi.yml
- filename: ireceipt-pro-png-api-openapi.yml
  format: yaml
  label: ireceipt-pro /png API
  slug: ireceipt-pro-png-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ireceipt-pro/openapi/ireceipt-pro-png-api-openapi.yml
- filename: ireceipt-pro-webp-api-openapi.yml
  format: yaml
  label: ireceipt-pro /webp API
  slug: ireceipt-pro-webp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ireceipt-pro/openapi/ireceipt-pro-webp-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ireceipt.pro
  spf: true
hosts:
- cert_expires: Jan 22 12:45:09 2027 GMT
  host: ireceipt.pro
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ireceipt Pro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ireceipt-pro, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ireceipt-pro
provider_slug: ireceipt-pro
slug: ireceipt-pro-domain-security
source_filename: ireceipt-pro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ireceipt.pro\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 12:45:09 2027 GMT\n  hsts: false\ndomains:\n- domain: ireceipt.pro\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/ireceipt-pro/security/ireceipt-pro-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- API
- PDF
- ImageGeneration
- Templates
---
