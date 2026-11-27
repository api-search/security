---
api_specs:
- filename: hermetics-fr-law-api-openapi.yml
  format: yaml
  label: Hermetics Law API
  slug: hermetics-fr-law-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hermetics-fr/openapi/hermetics-fr-law-api-openapi.yml
- filename: hermetics-fr-mcp-api-openapi.yml
  format: yaml
  label: Hermetics MCP API
  slug: hermetics-fr-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hermetics-fr/openapi/hermetics-fr-mcp-api-openapi.yml
- filename: hermetics-fr-records-api-openapi.yml
  format: yaml
  label: Hermetics Records API
  slug: hermetics-fr-records-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hermetics-fr/openapi/hermetics-fr-records-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hermetics.fr
  spf: true
hosts:
- cert_expires: Dec 24 14:29:33 2026 GMT
  host: hermetics.fr
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Hermetics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hermetics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Hermetics
provider_slug: hermetics-fr
slug: hermetics-fr-domain-security
source_filename: hermetics-fr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hermetics.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 14:29:33 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: hermetics.fr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/hermetics-fr/security/hermetics-fr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
---
