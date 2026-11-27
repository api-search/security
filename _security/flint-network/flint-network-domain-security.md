---
api_specs:
- filename: flint-network-agent-passport-api-openapi.yml
  format: yaml
  label: FLINT Network Agent Passport API
  slug: flint-network-agent-passport-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flint-network/openapi/flint-network-agent-passport-api-openapi.yml
- filename: flint-network-agent-sessions-api-openapi.yml
  format: yaml
  label: FLINT Network Agent Sessions API
  slug: flint-network-agent-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flint-network/openapi/flint-network-agent-sessions-api-openapi.yml
- filename: flint-network-outcome-feedback-api-openapi.yml
  format: yaml
  label: FLINT Network Outcome Feedback API
  slug: flint-network-outcome-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flint-network/openapi/flint-network-outcome-feedback-api-openapi.yml
- filename: flint-network-scout-credits-api-openapi.yml
  format: yaml
  label: FLINT Network Scout Credits API
  slug: flint-network-scout-credits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flint-network/openapi/flint-network-scout-credits-api-openapi.yml
- filename: flint-network-trust-graph-api-openapi.yml
  format: yaml
  label: FLINT Network Trust Graph API
  slug: flint-network-trust-graph-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flint-network/openapi/flint-network-trust-graph-api-openapi.yml
- filename: flint-network-verification-records-api-openapi.yml
  format: yaml
  label: FLINT Network Verification Records API
  slug: flint-network-verification-records-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flint-network/openapi/flint-network-verification-records-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: flint.network
  spf: false
hosts:
- cert_expires: Feb  3 13:57:31 2027 GMT
  host: flint.network
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: FLINT Network Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FLINT Network, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: FLINT Network
provider_slug: flint-network
slug: flint-network-domain-security
source_filename: flint-network-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flint.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 13:57:31 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: flint.network\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/flint-network/security/flint-network-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Fraud Prevention
- Compliance
- Agentic Commerce
- Real-Time
---
