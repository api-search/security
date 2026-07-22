---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: fab.com
  spf: false
hosts:
- cert_expires: Sep  5 13:29:22 2026 GMT
  host: www.fab.com
  hsts: true
  hsts_max_age: 604800
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fabcom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fab.com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Fab.com
provider_slug: fabcom
slug: fabcom-domain-security
source_filename: fabcom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fab.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 13:29:22 2026 GMT\n  hsts: true\n  hsts_max_age: 604800\ndomains:\n- domain: fab.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fabcom/refs/heads/main/security/fabcom-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Marketplace
- Digital Assets
- 3D Content
- Game Development
- Creator Economy
- Ecommerce
- Unreal Engine
- Epic Games
---
