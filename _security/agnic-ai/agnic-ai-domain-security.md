---
api_specs:
- filename: agnic-ai-api-reference-openapi-generated.yml
  format: yaml
  label: Agnic API Reference API
  slug: api-reference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agnic-ai/openapi/_ae-authored/agnic-ai-api-reference-openapi-generated.yml
- filename: agnic-ai-core-openapi-generated.yml
  format: yaml
  label: Agnic core API
  slug: core-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agnic-ai/openapi/_ae-authored/agnic-ai-core-openapi-generated.yml
- filename: agnic-ai-x402-openapi-generated.yml
  format: yaml
  label: Agnic X402 API
  slug: x402-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agnic-ai/openapi/_ae-authored/agnic-ai-x402-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: agnic.ai
  spf: true
hosts:
- cert_expires: Dec  4 02:26:30 2026 GMT
  host: agnic.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Agnic Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agnic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Agnic
provider_slug: agnic-ai
slug: agnic-ai-domain-security
source_filename: agnic-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agnic.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 02:26:30 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: agnic.ai\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/agnic-ai/security/agnic-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Agent Wallet
- Payment Infrastructure
- AI Commerce
- Verifiable Credentials
- API Monetization
- Service Discovery
---
