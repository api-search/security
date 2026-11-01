---
api_specs:
- filename: dxchange-openapi-generated.yml
  format: yaml
  label: DXchange.io API
  slug: dxchange-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dxchange/openapi/_ae-authored/dxchange-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dxchange.io
  spf: true
hosts:
- cert_expires: Nov 24 08:48:36 2026 GMT
  host: dxchange.io
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dxchange Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DXchange.io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: DXchange.io
provider_slug: dxchange
slug: dxchange-domain-security
source_filename: dxchange-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dxchange.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 08:48:36 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: dxchange.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/dxchange/security/dxchange-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Integration
- API Management
- Managed File Transfer
- B2B Integration
- Enterprise Data
---
