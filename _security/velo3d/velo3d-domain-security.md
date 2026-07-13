---
api_specs:
- filename: velo3d-openapi.yml
  format: yaml
  label: Velo3D Sapphire Printers
  slug: sapphire-printers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/velo3d/refs/heads/main/openapi/velo3d-openapi.yml
- filename: velo3d-openapi.yml
  format: yaml
  label: Velo3D Flow Print Preparation
  slug: flow-print-prep
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/velo3d/refs/heads/main/openapi/velo3d-openapi.yml
- filename: velo3d-openapi.yml
  format: yaml
  label: Velo3D Assure Quality Assurance
  slug: assure-qa
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/velo3d/refs/heads/main/openapi/velo3d-openapi.yml
- filename: velo3d-openapi.yml
  format: yaml
  label: Velo3D Intelligent Fusion
  slug: intelligent-fusion
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/velo3d/refs/heads/main/openapi/velo3d-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: velo3d.com
  spf: true
hosts:
- cert_expires: Aug 28 09:49:46 2026 GMT
  host: velo3d.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Velo3D Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Velo3D, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Velo3D
provider_slug: velo3d
slug: velo3d-domain-security
source_filename: velo3d-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: velo3d.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 09:49:46 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: velo3d.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/velo3d/refs/heads/main/security/velo3d-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Additive Manufacturing
- Metal 3D Printing
- Laser Powder Bed Fusion
- Aerospace
- Defense
---
