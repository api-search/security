---
api_specs:
- filename: capable-run-openapi-generated.yml
  format: yaml
  label: Capable API
  slug: capable-run-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capable-run/openapi/_ae-authored/capable-run-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: capable.run
  spf: true
hosts:
- cert_expires: Jan  8 20:08:10 2027 GMT
  host: capable.run
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Capable Run Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Capable, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Capable
provider_slug: capable-run
slug: capable-run-domain-security
source_filename: capable-run-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: capable.run\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 20:08:10 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: capable.run\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/capable-run/security/capable-run-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- CRM
- Artificial Intelligence
- MCP
- Software-as-a-Service
- Sales
---
