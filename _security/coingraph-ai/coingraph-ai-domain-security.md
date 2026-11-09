---
api_specs:
- filename: coingraph-ai-agents-api-openapi.yml
  format: yaml
  label: CoinGraph Agents API
  slug: coingraph-ai-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coingraph-ai/openapi/coingraph-ai-agents-api-openapi.yml
- filename: coingraph-ai-decide-api-openapi.yml
  format: yaml
  label: CoinGraph Decide API
  slug: coingraph-ai-decide-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coingraph-ai/openapi/coingraph-ai-decide-api-openapi.yml
- filename: coingraph-ai-discover-api-openapi.yml
  format: yaml
  label: CoinGraph Discover API
  slug: coingraph-ai-discover-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coingraph-ai/openapi/coingraph-ai-discover-api-openapi.yml
- filename: coingraph-ai-trust-api-openapi.yml
  format: yaml
  label: CoinGraph Trust API
  slug: coingraph-ai-trust-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coingraph-ai/openapi/coingraph-ai-trust-api-openapi.yml
- filename: coingraph-ai-understand-api-openapi.yml
  format: yaml
  label: CoinGraph Understand API
  slug: coingraph-ai-understand-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coingraph-ai/openapi/coingraph-ai-understand-api-openapi.yml
- filename: coingraph-ai-watch-api-openapi.yml
  format: yaml
  label: CoinGraph Watch API
  slug: coingraph-ai-watch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coingraph-ai/openapi/coingraph-ai-watch-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: coingraph.ai
  spf: true
hosts:
- cert_expires: Jan 17 05:36:22 2027 GMT
  host: coingraph.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Coingraph Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CoinGraph, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: CoinGraph
provider_slug: coingraph-ai
slug: coingraph-ai-domain-security
source_filename: coingraph-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: coingraph.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 05:36:22 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: coingraph.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/coingraph-ai/security/coingraph-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Crypto Data
- AI Agents
- trading agents
- Wallets
- On-Chain Data
- Market Data
---
