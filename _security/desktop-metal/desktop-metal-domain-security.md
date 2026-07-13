---
api_specs:
- filename: desktop-metal-openapi.yml
  format: yaml
  label: Printer Fleet & Live Suite
  slug: printer-fleet-live-suite
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/desktop-metal/refs/heads/main/openapi/desktop-metal-openapi.yml
- filename: desktop-metal-openapi.yml
  format: yaml
  label: Fabricate Software
  slug: fabricate-software
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/desktop-metal/refs/heads/main/openapi/desktop-metal-openapi.yml
- filename: desktop-metal-openapi.yml
  format: yaml
  label: Materials
  slug: materials
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/desktop-metal/refs/heads/main/openapi/desktop-metal-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: desktopmetal.com
  spf: true
hosts:
- cert_expires: Aug 16 08:56:50 2026 GMT
  host: www.desktopmetal.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Desktop Metal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Desktop Metal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Desktop Metal
provider_slug: desktop-metal
slug: desktop-metal-domain-security
source_filename: desktop-metal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.desktopmetal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 08:56:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: desktopmetal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/desktop-metal/refs/heads/main/security/desktop-metal-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- 3D Printing
- Additive Manufacturing
- Metal
- Hardware
- Manufacturing Software
---
