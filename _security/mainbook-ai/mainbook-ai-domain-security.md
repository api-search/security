---
api_specs:
- filename: mainbook-ai-developer-api-openapi.yml
  format: yaml
  label: MainBook Developer API
  slug: mainbook-ai-developer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mainbook-ai/openapi/mainbook-ai-developer-api-openapi.yml
- filename: mainbook-ai-device-authorization-api-openapi.yml
  format: yaml
  label: MainBook Device Authorization API
  slug: mainbook-ai-device-authorization-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mainbook-ai/openapi/mainbook-ai-device-authorization-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mainbook.ai
  spf: true
hosts:
- cert_expires: Dec 22 13:07:43 2026 GMT
  host: mainbook.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MainBook Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MainBook, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MainBook
provider_slug: mainbook-ai
slug: mainbook-ai-domain-security
source_filename: mainbook-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mainbook.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 13:07:43 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: mainbook.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/mainbook-ai/security/mainbook-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Bank Statement Conversion
- PDF to Excel
- Data Extraction
- Financial Data Processing
---
