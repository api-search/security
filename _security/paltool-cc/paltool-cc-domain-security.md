---
api_specs:
- filename: paltool-cc-openapi-generated.yml
  format: yaml
  label: PalTool API
  slug: paltool-cc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/paltool-cc/openapi/_ae-authored/paltool-cc-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: paltool.cc
  spf: true
hosts:
- cert_expires: Jan  5 15:01:17 2027 GMT
  host: paltool.cc
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: PalTool Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PalTool, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: PalTool
provider_slug: paltool-cc
slug: paltool-cc-domain-security
source_filename: paltool-cc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: paltool.cc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 15:01:17 2027 GMT\n  hsts: false\ndomains:\n- domain: paltool.cc\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/paltool-cc/security/paltool-cc-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Palworld
- Gaming
- Calculator
- Breeding
- Unofficial
---
