---
api_specs:
- filename: carrick-tools-openapi-generated.yml
  format: yaml
  label: Carrick API
  slug: carrick-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/carrick-tools/openapi/_ae-authored/carrick-tools-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: carrick.tools
  spf: true
hosts:
- cert_expires: Dec  8 23:40:25 2026 GMT
  host: carrick.tools
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Carrick Tools Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Carrick, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Carrick
provider_slug: carrick-tools
slug: carrick-tools-domain-security
source_filename: carrick-tools-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: carrick.tools\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 23:40:25 2026 GMT\n  hsts: false\ndomains:\n- domain: carrick.tools\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/carrick-tools/security/carrick-tools-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- TypeScript
- Code Intelligence
- Developer Tools
- Open Source
---
