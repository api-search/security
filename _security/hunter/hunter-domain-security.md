---
api_specs:
- filename: hunter-account-api-openapi.yml
  format: yaml
  label: Hunter Account API
  slug: hunter-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hunter/openapi/hunter-account-api-openapi.yml
- filename: hunter-campaigns-api-openapi.yml
  format: yaml
  label: Hunter Campaigns API
  slug: hunter-campaigns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hunter/openapi/hunter-campaigns-api-openapi.yml
- filename: hunter-discover-api-openapi.yml
  format: yaml
  label: Hunter Discover API
  slug: hunter-discover-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hunter/openapi/hunter-discover-api-openapi.yml
- filename: hunter-leads-api-openapi.yml
  format: yaml
  label: Hunter Leads API
  slug: hunter-leads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hunter/openapi/hunter-leads-api-openapi.yml
- filename: hunter-api-keys-api-openapi.yml
  format: yaml
  label: Hunter API Keys API
  slug: hunter-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hunter/openapi/hunter-api-keys-api-openapi.yml
- filename: hunter-companies-api-openapi.yml
  format: yaml
  label: Hunter Companies API
  slug: hunter-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hunter/openapi/hunter-companies-api-openapi.yml
- filename: hunter-connected-apps-api-openapi.yml
  format: yaml
  label: Hunter Connected Apps API
  slug: hunter-connected-apps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hunter/openapi/hunter-connected-apps-api-openapi.yml
- filename: hunter-email-accounts-api-openapi.yml
  format: yaml
  label: Hunter Email Accounts API
  slug: hunter-email-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hunter/openapi/hunter-email-accounts-api-openapi.yml
- filename: hunter-enrichment-api-openapi.yml
  format: yaml
  label: Hunter Enrichment API
  slug: hunter-enrichment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hunter/openapi/hunter-enrichment-api-openapi.yml
- filename: hunter-feedback-api-openapi.yml
  format: yaml
  label: Hunter Feedback API
  slug: hunter-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hunter/openapi/hunter-feedback-api-openapi.yml
- filename: hunter-finder-api-openapi.yml
  format: yaml
  label: Hunter Finder API
  slug: hunter-finder-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hunter/openapi/hunter-finder-api-openapi.yml
- filename: hunter-lists-api-openapi.yml
  format: yaml
  label: Hunter Lists API
  slug: hunter-lists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hunter/openapi/hunter-lists-api-openapi.yml
- filename: hunter-messages-api-openapi.yml
  format: yaml
  label: Hunter Messages API
  slug: hunter-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hunter/openapi/hunter-messages-api-openapi.yml
- filename: hunter-multi-domain-search-api-openapi.yml
  format: yaml
  label: Hunter Multi-Domain Search API
  slug: hunter-multi-domain-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hunter/openapi/hunter-multi-domain-search-api-openapi.yml
- filename: hunter-sequences-api-openapi.yml
  format: yaml
  label: Hunter Sequences API
  slug: hunter-sequences-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hunter/openapi/hunter-sequences-api-openapi.yml
- filename: hunter-tags-api-openapi.yml
  format: yaml
  label: Hunter Tags API
  slug: hunter-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hunter/openapi/hunter-tags-api-openapi.yml
- filename: hunter-team-api-openapi.yml
  format: yaml
  label: Hunter Team API
  slug: hunter-team-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hunter/openapi/hunter-team-api-openapi.yml
- filename: hunter-templates-api-openapi.yml
  format: yaml
  label: Hunter Templates API
  slug: hunter-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hunter/openapi/hunter-templates-api-openapi.yml
- filename: hunter-usage-api-openapi.yml
  format: yaml
  label: Hunter Usage API
  slug: hunter-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hunter/openapi/hunter-usage-api-openapi.yml
- filename: hunter-verifier-api-openapi.yml
  format: yaml
  label: Hunter Verifier API
  slug: hunter-verifier-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hunter/openapi/hunter-verifier-api-openapi.yml
- filename: hunter-views-api-openapi.yml
  format: yaml
  label: Hunter Views API
  slug: hunter-views-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hunter/openapi/hunter-views-api-openapi.yml
- filename: hunter-webhooks-api-openapi.yml
  format: yaml
  label: Hunter Webhooks API
  slug: hunter-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hunter/openapi/hunter-webhooks-api-openapi.yml
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
hosts_probed: 2
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
source_yaml_url: https://artifacts.apis.io/hunter/security/hunter-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Contact Discovery
- Email
- Email Verification
- Lead Generation
- Prospecting
- Sales Intelligence
---
