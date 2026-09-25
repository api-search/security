---
api_specs:
- filename: cracked-apps-api-openapi.yml
  format: yaml
  label: Cracked API Apps API
  slug: cracked-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cracked/refs/heads/main/openapi/cracked-apps-api-openapi.yml
- filename: cracked-auth-api-openapi.yml
  format: yaml
  label: Cracked API Auth API
  slug: cracked-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cracked/refs/heads/main/openapi/cracked-auth-api-openapi.yml
- filename: cracked-batches-api-openapi.yml
  format: yaml
  label: Cracked API Batches API
  slug: cracked-batches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cracked/refs/heads/main/openapi/cracked-batches-api-openapi.yml
- filename: cracked-datasets-api-openapi.yml
  format: yaml
  label: Cracked API Datasets API
  slug: cracked-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cracked/refs/heads/main/openapi/cracked-datasets-api-openapi.yml
- filename: cracked-discover-api-openapi.yml
  format: yaml
  label: Cracked API Discover API
  slug: cracked-discover-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cracked/refs/heads/main/openapi/cracked-discover-api-openapi.yml
- filename: cracked-inspect-api-openapi.yml
  format: yaml
  label: Cracked API Inspect API
  slug: cracked-inspect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cracked/refs/heads/main/openapi/cracked-inspect-api-openapi.yml
- filename: cracked-providers-api-openapi.yml
  format: yaml
  label: Cracked API Providers API
  slug: cracked-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cracked/refs/heads/main/openapi/cracked-providers-api-openapi.yml
- filename: cracked-referrals-api-openapi.yml
  format: yaml
  label: Cracked API Referrals API
  slug: cracked-referrals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cracked/refs/heads/main/openapi/cracked-referrals-api-openapi.yml
- filename: cracked-refunds-api-openapi.yml
  format: yaml
  label: Cracked API Refunds API
  slug: cracked-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cracked/refs/heads/main/openapi/cracked-refunds-api-openapi.yml
- filename: cracked-relay-api-openapi.yml
  format: yaml
  label: Cracked API Relay API
  slug: cracked-relay-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cracked/refs/heads/main/openapi/cracked-relay-api-openapi.yml
- filename: cracked-run-api-openapi.yml
  format: yaml
  label: Cracked API Run API
  slug: cracked-run-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cracked/refs/heads/main/openapi/cracked-run-api-openapi.yml
- filename: cracked-runs-api-openapi.yml
  format: yaml
  label: Cracked API Runs API
  slug: cracked-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cracked/refs/heads/main/openapi/cracked-runs-api-openapi.yml
- filename: cracked-schedules-api-openapi.yml
  format: yaml
  label: Cracked API Schedules API
  slug: cracked-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cracked/refs/heads/main/openapi/cracked-schedules-api-openapi.yml
- filename: cracked-secrets-api-openapi.yml
  format: yaml
  label: Cracked API Secrets API
  slug: cracked-secrets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cracked/refs/heads/main/openapi/cracked-secrets-api-openapi.yml
- filename: cracked-wallet-api-openapi.yml
  format: yaml
  label: Cracked API Wallet API
  slug: cracked-wallet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cracked/refs/heads/main/openapi/cracked-wallet-api-openapi.yml
- filename: cracked-x402-api-openapi.yml
  format: yaml
  label: Cracked API X402 API
  slug: cracked-x402-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cracked/refs/heads/main/openapi/cracked-x402-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cracked.ai
  spf: true
hosts:
- cert_expires: Dec  1 17:17:35 2026 GMT
  host: cracked.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cracked Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cracked API, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cracked API
provider_slug: cracked
slug: cracked-domain-security
source_filename: cracked-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cracked.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 17:17:35 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: cracked.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cracked/refs/heads/main/security/cracked-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Agents
- Agent Tools
- MCP
- Tool Router
- API Aggregator
- Web Search
- Web Scraping
- Data Enrichment
- llms-txt
- Agent Skills
- pay-per-call
- Aggregator
- Lead Generation
- AI Models
- Developer Tools
- lead gen
- SEO
- social-media-data
- E-Commerce
- Finance
- Weather
- A2A
---
