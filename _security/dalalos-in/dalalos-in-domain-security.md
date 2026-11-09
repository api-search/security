---
api_specs:
- filename: dalalos-in-openapi-generated.yml
  format: yaml
  label: DalalOS API
  slug: dalalos-in-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dalalos-in/openapi/_ae-authored/dalalos-in-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: dalalos.in
  spf: true
hosts:
- cert_expires: Jan 27 17:18:24 2027 GMT
  host: dalalos.in
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dalalos In Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DalalOS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: DalalOS
provider_slug: dalalos-in
slug: dalalos-in-domain-security
source_filename: dalalos-in-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dalalos.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 17:18:24 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dalalos.in\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/dalalos-in/security/dalalos-in-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Finance
- Data
- Artificial Intelligence
- Stock Market
- MCP
---
