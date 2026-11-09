---
api_specs:
- filename: agentrapay-ai-agents-api-openapi.yml
  format: yaml
  label: Agentra Agents API
  slug: agentrapay-ai-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentrapay-ai/openapi/agentrapay-ai-agents-api-openapi.yml
- filename: agentrapay-ai-authorizations-api-openapi.yml
  format: yaml
  label: Agentra Authorizations API
  slug: agentrapay-ai-authorizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentrapay-ai/openapi/agentrapay-ai-authorizations-api-openapi.yml
- filename: agentrapay-ai-health-api-openapi.yml
  format: yaml
  label: Agentra Health API
  slug: agentrapay-ai-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentrapay-ai/openapi/agentrapay-ai-health-api-openapi.yml
- filename: agentrapay-ai-trust-api-openapi.yml
  format: yaml
  label: Agentra Trust API
  slug: agentrapay-ai-trust-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentrapay-ai/openapi/agentrapay-ai-trust-api-openapi.yml
- filename: agentrapay-ai-wallets-api-openapi.yml
  format: yaml
  label: Agentra Wallets API
  slug: agentrapay-ai-wallets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentrapay-ai/openapi/agentrapay-ai-wallets-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: agentrapay.ai
  spf: true
hosts:
- cert_expires: Dec  2 15:12:20 2026 GMT
  host: agentrapay.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Agentrapay Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agentra, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Agentra
provider_slug: agentrapay-ai
slug: agentrapay-ai-domain-security
source_filename: agentrapay-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agentrapay.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 15:12:20 2026 GMT\n  hsts: false\ndomains:\n- domain: agentrapay.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/agentrapay-ai/security/agentrapay-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Identity Verification
- Reputation Scoring
- Transaction Authorization
- Non‑Custodial Wallet
- Agent Infrastructure
---
