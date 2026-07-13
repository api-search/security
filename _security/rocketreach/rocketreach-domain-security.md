---
api_specs:
- filename: rocketreach-people-lookup-api-openapi.yml
  format: yaml
  label: RocketReach People Lookup API
  slug: rocketreach-people-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rocketreach/refs/heads/main/openapi/rocketreach-people-lookup-api-openapi.yml
- filename: rocketreach-people-search-api-openapi.yml
  format: yaml
  label: RocketReach People Search API
  slug: rocketreach-people-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rocketreach/refs/heads/main/openapi/rocketreach-people-search-api-openapi.yml
- filename: rocketreach-company-lookup-api-openapi.yml
  format: yaml
  label: RocketReach Company Lookup API
  slug: rocketreach-company-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rocketreach/refs/heads/main/openapi/rocketreach-company-lookup-api-openapi.yml
- filename: rocketreach-company-search-api-openapi.yml
  format: yaml
  label: RocketReach Company Search API
  slug: rocketreach-company-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rocketreach/refs/heads/main/openapi/rocketreach-company-search-api-openapi.yml
- filename: rocketreach-account-api-openapi.yml
  format: yaml
  label: RocketReach Account API
  slug: rocketreach-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rocketreach/refs/heads/main/openapi/rocketreach-account-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: rocketreach.co
  spf: true
hosts:
- cert_expires: Sep 14 18:46:00 2026 GMT
  host: rocketreach.co
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 16 01:32:43 2026 GMT
  host: docs.rocketreach.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 18:46:00 2026 GMT
  host: api.rocketreach.co
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rocketreach Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RocketReach, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: RocketReach
provider_slug: rocketreach
slug: rocketreach-domain-security
source_filename: rocketreach-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rocketreach.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 18:46:00 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: docs.rocketreach.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 01:32:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.rocketreach.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 18:46:00 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: rocketreach.co\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rocketreach/refs/heads/main/security/rocketreach-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- B2B
- Contact Data
- Email Lookup
- Phone Lookup
- Sales Intelligence
- Lead Generation
- People Search
- Company Search
- Data Enrichment
- Prospecting
- Recruiting
- Webhooks
---
