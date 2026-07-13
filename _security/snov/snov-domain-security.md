---
api_specs:
- filename: snov-openapi.yml
  format: yaml
  label: Snov.io Authentication API
  slug: snov-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov/refs/heads/main/openapi/snov-openapi.yml
- filename: snov-openapi.yml
  format: yaml
  label: Snov.io Email Finder API
  slug: snov-email-finder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov/refs/heads/main/openapi/snov-openapi.yml
- filename: snov-openapi.yml
  format: yaml
  label: Snov.io Domain Search API
  slug: snov-domain-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov/refs/heads/main/openapi/snov-openapi.yml
- filename: snov-openapi.yml
  format: yaml
  label: Snov.io Email Verifier API
  slug: snov-email-verifier-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov/refs/heads/main/openapi/snov-openapi.yml
- filename: snov-openapi.yml
  format: yaml
  label: Snov.io Enrichment API
  slug: snov-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov/refs/heads/main/openapi/snov-openapi.yml
- filename: snov-openapi.yml
  format: yaml
  label: Snov.io Prospects & Lists API
  slug: snov-prospects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov/refs/heads/main/openapi/snov-openapi.yml
- filename: snov-openapi.yml
  format: yaml
  label: Snov.io Drip Campaigns API
  slug: snov-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov/refs/heads/main/openapi/snov-openapi.yml
- filename: snov-openapi.yml
  format: yaml
  label: Snov.io Sender Accounts API
  slug: snov-sender-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov/refs/heads/main/openapi/snov-openapi.yml
- filename: snov-openapi.yml
  format: yaml
  label: Snov.io Email Warm-up API
  slug: snov-warmup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov/refs/heads/main/openapi/snov-openapi.yml
- filename: snov-openapi.yml
  format: yaml
  label: Snov.io User & Balance API
  slug: snov-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov/refs/heads/main/openapi/snov-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: snov.io
  spf: true
hosts:
- cert_expires: Oct 10 23:59:59 2026 GMT
  host: snov.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 23:59:59 2026 GMT
  host: api.snov.io
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Snov Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Snov.io, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Snov.io
provider_slug: snov
slug: snov-domain-security
source_filename: snov-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: snov.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.snov.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  5 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: snov.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/snov/refs/heads/main/security/snov-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Sales Engagement
- Email Finder
- Email Verification
- Prospecting
- Drip Campaigns
- CRM
- Lead Generation
---
