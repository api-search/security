---
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
name: Looking Glass Factory Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Looking Glass Factory, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Looking Glass Factory
provider_slug: looking-glass-factory
slug: looking-glass-factory-domain-security
source_filename: looking-glass-factory-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lookingglassfactory.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 11:23:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lookingglassfactory.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/looking-glass-factory/refs/heads/main/security/looking-glass-factory-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Hardware
- Holographic Displays
- 3D
- Light Field
- Developer Tools
- SDK
- GraphQL
- WebXR
- AR VR
---
