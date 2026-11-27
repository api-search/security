---
api_specs:
- filename: agentik-cc-discover-api-openapi.yml
  format: yaml
  label: Agentik Discover API
  slug: agentik-cc-discover-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentik-cc/openapi/agentik-cc-discover-api-openapi.yml
- filename: agentik-cc-oauth-api-openapi.yml
  format: yaml
  label: Agentik OAuth API
  slug: agentik-cc-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentik-cc/openapi/agentik-cc-oauth-api-openapi.yml
- filename: agentik-cc-run-api-openapi.yml
  format: yaml
  label: Agentik Run API
  slug: agentik-cc-run-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentik-cc/openapi/agentik-cc-run-api-openapi.yml
- filename: agentik-cc-wallet-api-openapi.yml
  format: yaml
  label: Agentik Wallet API
  slug: agentik-cc-wallet-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentik-cc/openapi/agentik-cc-wallet-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: agentik.cc
  spf: true
hosts:
- cert_expires: Dec 15 09:45:43 2026 GMT
  host: www.agentik.cc
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Agentik Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agentik, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Agentik
provider_slug: agentik-cc
slug: agentik-cc-domain-security
source_filename: agentik-cc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.agentik.cc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 09:45:43 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: agentik.cc\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/agentik-cc/security/agentik-cc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Automation
- Tools
- MCP
- Software-as-a-Service
---
