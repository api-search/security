---
api_specs:
- filename: surfe-b2b-openapi.yml
  format: yaml
  label: Surfe People Enrichment API
  slug: surfe-b2b-people-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/surfe-b2b/refs/heads/main/openapi/surfe-b2b-openapi.yml
- filename: surfe-b2b-openapi.yml
  format: yaml
  label: Surfe People Search API
  slug: surfe-b2b-people-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/surfe-b2b/refs/heads/main/openapi/surfe-b2b-openapi.yml
- filename: surfe-b2b-openapi.yml
  format: yaml
  label: Surfe Company Enrichment API
  slug: surfe-b2b-company-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/surfe-b2b/refs/heads/main/openapi/surfe-b2b-openapi.yml
- filename: surfe-b2b-openapi.yml
  format: yaml
  label: Surfe Company Search API
  slug: surfe-b2b-company-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/surfe-b2b/refs/heads/main/openapi/surfe-b2b-openapi.yml
- filename: surfe-b2b-openapi.yml
  format: yaml
  label: Surfe Credits API
  slug: surfe-b2b-credits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/surfe-b2b/refs/heads/main/openapi/surfe-b2b-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: surfe.com
  spf: true
hosts:
- cert_expires: Aug 24 07:04:33 2026 GMT
  host: developers.surfe.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 18:57:27 2026 GMT
  host: api.surfe.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Surfe B2B Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Surfe, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Surfe
provider_slug: surfe-b2b
slug: surfe-b2b-domain-security
source_filename: surfe-b2b-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.surfe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 07:04:33 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.surfe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 18:57:27 2026 GMT\n  hsts: null\ndomains:\n- domain: surfe.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/surfe-b2b/refs/heads/main/security/surfe-b2b-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Contact Discovery
- Data Enrichment
- B2B Data
- Sales Intelligence
- Lead Enrichment
- Web Intelligence
- Contact Data
- People Enrichment
- Company Enrichment
- Prospecting
---
