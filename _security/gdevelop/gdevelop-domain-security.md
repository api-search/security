---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gdevelop.io
  spf: true
hosts:
- cert_expires: Oct  3 18:58:28 2026 GMT
  host: gdevelop.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gdevelop Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GDevelop, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: GDevelop
provider_slug: gdevelop
slug: gdevelop-domain-security
source_filename: gdevelop-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gdevelop.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 18:58:28 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: gdevelop.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gdevelop/refs/heads/main/security/gdevelop-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Game Engine
- Game Development
- No-Code
- Open Source
- Developer Tools
- Cross-Platform
- Multiplayer
---
