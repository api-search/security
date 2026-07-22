---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bricks.tools
  spf: true
hosts:
- cert_expires: Oct  7 16:20:16 2026 GMT
  host: bricks.tools
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bricks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BRICKS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: BRICKS
provider_slug: bricks
slug: bricks-domain-security
source_filename: bricks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bricks.tools\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 16:20:16 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: bricks.tools\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bricks/refs/heads/main/security/bricks-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Digital Signage
- Kiosk
- No-Code
- Interactive Displays
- PaaS
- Content Management
- Screens
---
