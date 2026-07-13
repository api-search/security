---
api_specs:
- filename: hunter-api-openapi.yml
  format: yaml
  label: Hunter Domain Search API
  slug: domain-search
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-api-openapi.yml
- filename: hunter-api-openapi.yml
  format: yaml
  label: Hunter Email Finder API
  slug: email-finder
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-api-openapi.yml
- filename: hunter-api-openapi.yml
  format: yaml
  label: Hunter Email Verifier API
  slug: email-verifier
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-api-openapi.yml
- filename: hunter-api-openapi.yml
  format: yaml
  label: Hunter Email Count API
  slug: email-count
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-api-openapi.yml
- filename: hunter-api-openapi.yml
  format: yaml
  label: Hunter Account API
  slug: account
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-api-openapi.yml
- filename: hunter-api-openapi.yml
  format: yaml
  label: Hunter Discover API
  slug: discover
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-api-openapi.yml
- filename: hunter-api-openapi.yml
  format: yaml
  label: Hunter Email Enrichment API
  slug: email-enrichment
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-api-openapi.yml
- filename: hunter-api-openapi.yml
  format: yaml
  label: Hunter Company Enrichment API
  slug: company-enrichment
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-api-openapi.yml
- filename: hunter-api-openapi.yml
  format: yaml
  label: Hunter Combined Enrichment API
  slug: combined-enrichment
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-api-openapi.yml
- filename: hunter-api-openapi.yml
  format: yaml
  label: Hunter Leads API
  slug: leads
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-api-openapi.yml
- filename: hunter-api-openapi.yml
  format: yaml
  label: Hunter Leads Lists API
  slug: leads-lists
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-api-openapi.yml
- filename: hunter-api-openapi.yml
  format: yaml
  label: Hunter Campaigns API
  slug: campaigns
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-api-openapi.yml
- filename: hunter-api-openapi.yml
  format: yaml
  label: Hunter Logo API
  slug: logo
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: hunter.io
  spf: true
hosts:
- cert_expires: Sep 11 09:50:49 2026 GMT
  host: hunter.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 14 03:14:32 2026 GMT
  host: api.hunter.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 20:29:51 2026 GMT
  host: logos.hunter.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hunter Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hunter, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Hunter
provider_slug: hunter
slug: hunter-domain-security
source_filename: hunter-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hunter.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 09:50:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.hunter.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 03:14:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: logos.hunter.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 20:29:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hunter.io\n  dnssec: true\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
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
