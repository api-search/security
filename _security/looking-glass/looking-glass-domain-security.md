---
api_specs:
- filename: looking-glass-bridge-openapi.yml
  format: yaml
  label: Looking Glass Bridge API
  slug: looking-glass-bridge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/looking-glass/refs/heads/main/openapi/looking-glass-bridge-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: lookingglassfactory.com
  spf: true
hosts:
- cert_expires: Oct 16 11:23:07 2026 GMT
  host: lookingglassfactory.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Looking Glass Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Looking Glass, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Looking Glass
provider_slug: looking-glass
slug: looking-glass-domain-security
source_filename: looking-glass-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lookingglassfactory.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 11:23:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lookingglassfactory.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/looking-glass/refs/heads/main/security/looking-glass-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Holographic Displays
- Light Field
- 3D
- Developer Tools
- WebXR
- Hardware
- Holograms
- Media Player
---
