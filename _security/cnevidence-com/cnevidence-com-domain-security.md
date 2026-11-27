---
api_specs:
- filename: cnevidence-com-free-api-openapi.yml
  format: yaml
  label: CN Evidence Free API
  slug: cnevidence-com-free-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cnevidence-com/openapi/cnevidence-com-free-api-openapi.yml
- filename: cnevidence-com-x402-api-openapi.yml
  format: yaml
  label: CN Evidence X402 API
  slug: cnevidence-com-x402-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cnevidence-com/openapi/cnevidence-com-x402-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cnevidence.com
  spf: true
hosts:
- cert_expires: Dec 12 15:31:28 2026 GMT
  host: cnevidence.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: CN Evidence Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CN Evidence, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CN Evidence
provider_slug: cnevidence-com
slug: cnevidence-com-domain-security
source_filename: cnevidence-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cnevidence.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 15:31:28 2026 GMT\n  hsts: false\ndomains:\n- domain: cnevidence.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/cnevidence-com/security/cnevidence-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- China
- Company Data
- Due Diligence
- Supplier Screening
- KYB
- x402
- Payments
- MCP
- Business Information
---
