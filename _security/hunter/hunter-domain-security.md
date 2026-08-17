---
api_specs:
- filename: hunter-account-api-openapi.yml
  format: yaml
  label: Hunter Account API
  slug: hunter-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-account-api-openapi.yml
- filename: hunter-campaigns-api-openapi.yml
  format: yaml
  label: Hunter Campaigns API
  slug: hunter-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-campaigns-api-openapi.yml
- filename: hunter-combined-enrichment-api-openapi.yml
  format: yaml
  label: Hunter Combined Enrichment API
  slug: hunter-combined-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-combined-enrichment-api-openapi.yml
- filename: hunter-company-enrichment-api-openapi.yml
  format: yaml
  label: Hunter Company Enrichment API
  slug: hunter-company-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-company-enrichment-api-openapi.yml
- filename: hunter-discover-api-openapi.yml
  format: yaml
  label: Hunter Discover API
  slug: hunter-discover-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-discover-api-openapi.yml
- filename: hunter-domain-search-api-openapi.yml
  format: yaml
  label: Hunter Domain Search API
  slug: hunter-domain-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-domain-search-api-openapi.yml
- filename: hunter-email-count-api-openapi.yml
  format: yaml
  label: Hunter Email Count API
  slug: hunter-email-count-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-email-count-api-openapi.yml
- filename: hunter-email-enrichment-api-openapi.yml
  format: yaml
  label: Hunter Email Enrichment API
  slug: hunter-email-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-email-enrichment-api-openapi.yml
- filename: hunter-email-finder-api-openapi.yml
  format: yaml
  label: Hunter Email Finder API
  slug: hunter-email-finder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-email-finder-api-openapi.yml
- filename: hunter-email-verifier-api-openapi.yml
  format: yaml
  label: Hunter Email Verifier API
  slug: hunter-email-verifier-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-email-verifier-api-openapi.yml
- filename: hunter-leads-api-openapi.yml
  format: yaml
  label: Hunter Leads API
  slug: hunter-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-leads-api-openapi.yml
- filename: hunter-leads-lists-api-openapi.yml
  format: yaml
  label: Hunter Leads Lists API
  slug: hunter-leads-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-leads-lists-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: hunter.io
  spf: true
hosts:
- cert_expires: Nov  9 09:37:53 2026 GMT
  host: hunter.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 05:26:20 2026 GMT
  host: api.hunter.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hunter Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hunter, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Hunter
provider_slug: hunter
slug: hunter-domain-security
source_filename: hunter-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hunter.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 09:37:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.hunter.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 05:26:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hunter.io\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/security/hunter-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Contact Discovery
- Email
- Email Verification
- Lead Generation
- Prospecting
- Sales Intelligence
---
