---
api_specs:
- filename: crimp-studio-openapi-generated.yml
  format: yaml
  label: Crimp API
  slug: crimp-studio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crimp-studio/openapi/_ae-authored/crimp-studio-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: crimp.studio
  spf: true
hosts:
- cert_expires: Jan 31 02:32:52 2027 GMT
  host: crimp.studio
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Crimp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Crimp, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Crimp
provider_slug: crimp-studio
slug: crimp-studio-domain-security
source_filename: crimp-studio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: crimp.studio\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 02:32:52 2027 GMT\n  hsts: false\ndomains:\n- domain: crimp.studio\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/crimp-studio/security/crimp-studio-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Wiring Diagram Software
- 12V Systems
- Marine Electrical
- Campervan
- Off-Grid
- Electrical Simulation
---
