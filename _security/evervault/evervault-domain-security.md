---
api_specs:
- filename: evervault-3d-secure-api-openapi.yml
  format: yaml
  label: Evervault 3D Secure API
  slug: evervault-3d-secure-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evervault/refs/heads/main/openapi/evervault-3d-secure-api-openapi.yml
- filename: evervault-acquirers-api-openapi.yml
  format: yaml
  label: Evervault Acquirers API
  slug: evervault-acquirers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evervault/refs/heads/main/openapi/evervault-acquirers-api-openapi.yml
- filename: evervault-card-account-updates-api-openapi.yml
  format: yaml
  label: Evervault Card Account Updates API
  slug: evervault-card-account-updates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evervault/refs/heads/main/openapi/evervault-card-account-updates-api-openapi.yml
- filename: evervault-client-tokens-api-openapi.yml
  format: yaml
  label: Evervault Client Tokens API
  slug: evervault-client-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evervault/refs/heads/main/openapi/evervault-client-tokens-api-openapi.yml
- filename: evervault-core-api-openapi.yml
  format: yaml
  label: Evervault Core API
  slug: evervault-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evervault/refs/heads/main/openapi/evervault-core-api-openapi.yml
- filename: evervault-functions-api-openapi.yml
  format: yaml
  label: Evervault Functions API
  slug: evervault-functions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evervault/refs/heads/main/openapi/evervault-functions-api-openapi.yml
- filename: evervault-insights-api-openapi.yml
  format: yaml
  label: Evervault Insights API
  slug: evervault-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evervault/refs/heads/main/openapi/evervault-insights-api-openapi.yml
- filename: evervault-merchants-api-openapi.yml
  format: yaml
  label: Evervault Merchants API
  slug: evervault-merchants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evervault/refs/heads/main/openapi/evervault-merchants-api-openapi.yml
- filename: evervault-network-tokens-api-openapi.yml
  format: yaml
  label: Evervault Network Tokens API
  slug: evervault-network-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evervault/refs/heads/main/openapi/evervault-network-tokens-api-openapi.yml
- filename: evervault-payments-api-openapi.yml
  format: yaml
  label: Evervault Payments API
  slug: evervault-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evervault/refs/heads/main/openapi/evervault-payments-api-openapi.yml
- filename: evervault-relays-api-openapi.yml
  format: yaml
  label: Evervault Relays API
  slug: evervault-relays-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evervault/refs/heads/main/openapi/evervault-relays-api-openapi.yml
- filename: evervault-webhooks-api-openapi.yml
  format: yaml
  label: Evervault Webhooks API
  slug: evervault-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evervault/refs/heads/main/openapi/evervault-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: evervault.com
  spf: true
hosts:
- cert_expires: Sep 25 14:56:16 2026 GMT
  host: evervault.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Evervault Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Evervault, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Evervault
provider_slug: evervault
slug: evervault-domain-security
source_filename: evervault-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: evervault.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 14:56:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: evervault.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/evervault/refs/heads/main/security/evervault-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Data
- Security
- Encryption
- Payments
- PCI Compliance
- Tokenization
- Cards
- Developer Tools
---
