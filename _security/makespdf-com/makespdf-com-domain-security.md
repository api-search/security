---
api_specs:
- filename: makespdf-com-artifacts-api-openapi.yml
  format: yaml
  label: makespdf-com Artifacts API
  slug: makespdf-com-artifacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/makespdf-com/openapi/makespdf-com-artifacts-api-openapi.yml
- filename: makespdf-com-public-api-openapi.yml
  format: yaml
  label: makespdf-com Public API
  slug: makespdf-com-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/makespdf-com/openapi/makespdf-com-public-api-openapi.yml
- filename: makespdf-com-render-api-openapi.yml
  format: yaml
  label: makespdf-com Render API
  slug: makespdf-com-render-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/makespdf-com/openapi/makespdf-com-render-api-openapi.yml
- filename: makespdf-com-validate-api-openapi.yml
  format: yaml
  label: makespdf-com Validate API
  slug: makespdf-com-validate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/makespdf-com/openapi/makespdf-com-validate-api-openapi.yml
- filename: makespdf-com-x402-api-openapi.yml
  format: yaml
  label: makespdf-com X402 API
  slug: makespdf-com-x402-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/makespdf-com/openapi/makespdf-com-x402-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: makespdf.com
  spf: true
hosts:
- cert_expires: Jan 17 05:26:32 2027 GMT
  host: makespdf.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Makespdf Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for makespdf-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: makespdf-com
provider_slug: makespdf-com
slug: makespdf-com-domain-security
source_filename: makespdf-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: makespdf.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 05:26:32 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: makespdf.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/makespdf-com/security/makespdf-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- PDF
- API
- Conversion
- Developer
---
