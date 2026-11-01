---
api_specs:
- filename: llcdrop-account-api-openapi.yml
  format: yaml
  label: LLCDrop Account API
  slug: llcdrop-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/llcdrop/openapi/llcdrop-account-api-openapi.yml
- filename: llcdrop-businesses-api-openapi.yml
  format: yaml
  label: LLCDrop Businesses API
  slug: llcdrop-businesses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/llcdrop/openapi/llcdrop-businesses-api-openapi.yml
- filename: llcdrop-counties-and-stats-api-openapi.yml
  format: yaml
  label: LLCDrop Counties and stats API
  slug: llcdrop-counties-and-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/llcdrop/openapi/llcdrop-counties-and-stats-api-openapi.yml
- filename: llcdrop-datasets-api-openapi.yml
  format: yaml
  label: LLCDrop Datasets API
  slug: llcdrop-datasets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/llcdrop/openapi/llcdrop-datasets-api-openapi.yml
- filename: llcdrop-filings-api-openapi.yml
  format: yaml
  label: LLCDrop Filings API
  slug: llcdrop-filings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/llcdrop/openapi/llcdrop-filings-api-openapi.yml
- filename: llcdrop-parcels-api-openapi.yml
  format: yaml
  label: LLCDrop Parcels API
  slug: llcdrop-parcels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/llcdrop/openapi/llcdrop-parcels-api-openapi.yml
- filename: llcdrop-reference-lists-api-openapi.yml
  format: yaml
  label: LLCDrop Reference lists API
  slug: llcdrop-reference-lists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/llcdrop/openapi/llcdrop-reference-lists-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: llcdrop.com
  spf: true
hosts:
- cert_expires: Dec 23 08:37:57 2026 GMT
  host: llcdrop.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Llcdrop Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LLCDrop, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: LLCDrop
provider_slug: llcdrop
slug: llcdrop-domain-security
source_filename: llcdrop-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: llcdrop.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 08:37:57 2026 GMT\n  hsts: null\ndomains:\n- domain: llcdrop.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/llcdrop/security/llcdrop-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- lead-generation
- business-data
- marketing
- real-estate
- api
---
