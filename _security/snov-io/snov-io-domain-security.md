---
api_specs:
- filename: snov-io-email-verification-api-openapi.yml
  format: yaml
  label: Snov.io Email Verification API
  slug: snovio-email-verification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snov-io/openapi/snov-io-email-verification-api-openapi.yml
- filename: snov-io-campaigns-api-openapi.yml
  format: yaml
  label: Snov.io Campaigns API
  slug: snovio-campaigns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snov-io/openapi/snov-io-campaigns-api-openapi.yml
- filename: snov-io-email-warm-up-api-openapi.yml
  format: yaml
  label: Snov.io Email Warm-up API
  slug: snovio-email-warm-up-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snov-io/openapi/snov-io-email-warm-up-api-openapi.yml
- filename: snov-io-webhooks-api-openapi.yml
  format: yaml
  label: Snov.io Webhooks API
  slug: snovio-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snov-io/openapi/snov-io-webhooks-api-openapi.yml
- filename: snov-io-openapi-generated.yml
  format: yaml
  label: Snov.io API
  slug: snov-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snov-io/openapi/_ae-authored/snov-io-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: snov.io
  spf: true
hosts:
- cert_expires: Mar 12 23:59:59 2027 GMT
  host: snov.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  7 23:59:59 2027 GMT
  host: api.snov.io
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan 21 11:59:43 2027 GMT
  host: mcp.snov.io
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Snov.io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Snov.io, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Snov.io
provider_slug: snov-io
slug: snov-io-domain-security
source_filename: snov-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: snov.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 12 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.snov.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar  7 23:59:59 2027 GMT\n  hsts: null\n- host: mcp.snov.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 11:59:43 2027 GMT\n  hsts: null\ndomains:\n- domain: snov.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/snov-io/security/snov-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Sales Automation
- Email Finder
- Email Verification
- Lead Generation
- Drip Campaigns
- CRM
- LinkedIn Automation
- Prospect Management
- Data Enrichment
- Cold Email
---
