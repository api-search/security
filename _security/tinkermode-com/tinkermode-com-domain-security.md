---
api_specs:
- filename: tinkermode-com-openapi-generated.yml
  format: yaml
  label: Mode API
  slug: tinkermode-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tinkermode-com/openapi/_ae-authored/tinkermode-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tinkermode.com
  spf: true
hosts:
- cert_expires: Jan 30 23:59:59 2027 GMT
  host: tinkermode.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Tinkermode Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mode, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Mode
provider_slug: tinkermode-com
slug: tinkermode-com-domain-security
source_filename: tinkermode-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tinkermode.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: tinkermode.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/tinkermode-com/security/tinkermode-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI
- Data-Platform
- Industrial
- Construction
- Operations
- Company
---
