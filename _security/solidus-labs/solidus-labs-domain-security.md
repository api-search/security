---
api_specs:
- filename: solidus-labs-address-api-api-openapi.yml
  format: yaml
  label: Solidus Labs Address API API
  slug: solidus-labs-address-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solidus-labs/refs/heads/main/openapi/solidus-labs-address-api-api-openapi.yml
- filename: solidus-labs-chain-api-api-openapi.yml
  format: yaml
  label: Solidus Labs Chain API API
  slug: solidus-labs-chain-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solidus-labs/refs/heads/main/openapi/solidus-labs-chain-api-api-openapi.yml
- filename: solidus-labs-corrections-api-openapi.yml
  format: yaml
  label: Solidus Labs Corrections API
  slug: solidus-labs-corrections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solidus-labs/refs/heads/main/openapi/solidus-labs-corrections-api-openapi.yml
- filename: solidus-labs-latest-api-openapi.yml
  format: yaml
  label: Solidus Labs Latest API
  slug: solidus-labs-latest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solidus-labs/refs/heads/main/openapi/solidus-labs-latest-api-openapi.yml
- filename: solidus-labs-scams-api-openapi.yml
  format: yaml
  label: Solidus Labs Scams API
  slug: solidus-labs-scams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solidus-labs/refs/heads/main/openapi/solidus-labs-scams-api-openapi.yml
- filename: solidus-labs-token-api-api-openapi.yml
  format: yaml
  label: Solidus Labs Token API API
  slug: solidus-labs-token-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solidus-labs/refs/heads/main/openapi/solidus-labs-token-api-api-openapi.yml
- filename: solidus-labs-webhooks-api-api-openapi.yml
  format: yaml
  label: Solidus Labs Webhooks API API
  slug: solidus-labs-webhooks-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solidus-labs/refs/heads/main/openapi/solidus-labs-webhooks-api-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: soliduslabs.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: readme.io
  spf: true
hosts:
- cert_expires: Oct 14 10:15:50 2026 GMT
  host: www.soliduslabs.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 13:12:37 2026 GMT
  host: tokensniffer.readme.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 19:58:57 2026 GMT
  host: tokensniffer.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Solidus Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Solidus Labs, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Solidus Labs
provider_slug: solidus-labs
slug: solidus-labs-domain-security
source_filename: solidus-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.soliduslabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 10:15:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: tokensniffer.readme.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 13:12:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: tokensniffer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 19:58:57 2026 GMT\n  hsts: null\ndomains:\n- domain: soliduslabs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: readme.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/solidus-labs/refs/heads/main/security/solidus-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Compliance
- RegTech
- Trade Surveillance
- Market Integrity
- Transaction Monitoring
- Digital Assets
- Cryptocurrency
- Blockchain
- Token Security
- Scam Detection
- Smart Contracts
- Anti-Money Laundering
- Web3
- DeFi
---
