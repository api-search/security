---
api_specs:
- filename: boncourant-fr-audit-api-openapi.yml
  format: yaml
  label: Boncourant Audit API
  slug: boncourant-fr-audit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/boncourant-fr/openapi/boncourant-fr-audit-api-openapi.yml
- filename: boncourant-fr-commissions-api-openapi.yml
  format: yaml
  label: Boncourant Commissions API
  slug: boncourant-fr-commissions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/boncourant-fr/openapi/boncourant-fr-commissions-api-openapi.yml
- filename: boncourant-fr-mcp-api-openapi.yml
  format: yaml
  label: Boncourant MCP API
  slug: boncourant-fr-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/boncourant-fr/openapi/boncourant-fr-mcp-api-openapi.yml
- filename: boncourant-fr-simulate-api-openapi.yml
  format: yaml
  label: Boncourant Simulate API
  slug: boncourant-fr-simulate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/boncourant-fr/openapi/boncourant-fr-simulate-api-openapi.yml
- filename: boncourant-fr-trv-gap-api-openapi.yml
  format: yaml
  label: Boncourant Trv Gap API
  slug: boncourant-fr-trv-gap-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/boncourant-fr/openapi/boncourant-fr-trv-gap-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: boncourant.fr
  spf: true
hosts:
- cert_expires: Dec 25 19:02:20 2026 GMT
  host: boncourant.fr
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Boncourant Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Boncourant, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Boncourant
provider_slug: boncourant-fr
slug: boncourant-fr-domain-security
source_filename: boncourant-fr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: boncourant.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 19:02:20 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: boncourant.fr\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/boncourant-fr/security/boncourant-fr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Electricity
- Audit
- Optimization
- France
- Independent
---
