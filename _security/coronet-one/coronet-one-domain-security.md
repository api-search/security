---
api_specs:
- filename: coronet-one-confirm-checkout-api-openapi.yml
  format: yaml
  label: Coronet Arcade Confirm Checkout API
  slug: coronet-one-confirm-checkout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coronet-one/openapi/coronet-one-confirm-checkout-api-openapi.yml
- filename: coronet-one-create-checkout-api-openapi.yml
  format: yaml
  label: Coronet Arcade Create Checkout API
  slug: coronet-one-create-checkout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coronet-one/openapi/coronet-one-create-checkout-api-openapi.yml
- filename: coronet-one-mcp-api-openapi.yml
  format: yaml
  label: Coronet Arcade MCP API
  slug: coronet-one-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coronet-one/openapi/coronet-one-mcp-api-openapi.yml
- filename: coronet-one-restore-purchase-api-openapi.yml
  format: yaml
  label: Coronet Arcade Restore Purchase API
  slug: coronet-one-restore-purchase-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coronet-one/openapi/coronet-one-restore-purchase-api-openapi.yml
- filename: coronet-one-site-api-openapi.yml
  format: yaml
  label: Coronet Arcade Site API
  slug: coronet-one-site-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coronet-one/openapi/coronet-one-site-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: coronet.one
  spf: true
hosts:
- cert_expires: Jan 22 23:35:36 2027 GMT
  host: coronet.one
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Coronet Arcade Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coronet Arcade, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Coronet Arcade
provider_slug: coronet-one
slug: coronet-one-domain-security
source_filename: coronet-one-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: coronet.one\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 23:35:36 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: coronet.one\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/coronet-one/security/coronet-one-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Games
- Puzzles
- Word Games
- Logic Puzzles
- MCP
- AI Agents
---
