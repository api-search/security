---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: voxelenergy.com
  spf: false
hosts:
- cert_expires: Aug 26 00:36:05 2026 GMT
  host: www.voxelenergy.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Voxel Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Voxel Energy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Voxel Energy
provider_slug: voxel-energy
slug: voxel-energy-domain-security
source_filename: voxel-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.voxelenergy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 00:36:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: voxelenergy.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/voxel-energy/refs/heads/main/security/voxel-energy-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Data Centers
- Energy
- Solar Power
- Renewable Energy
- Batteries
- Hardware
- Infrastructure
- Artificial Intelligence
---
