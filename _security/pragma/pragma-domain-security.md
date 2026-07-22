---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pragma.gg
  spf: true
- caa:
  - ;; connection timed out; no servers could be reached
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: firstlook.gg
  spf: true
hosts:
- cert_expires: Jan 28 23:59:59 2027 GMT
  host: pragma.gg
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 22:09:00 2026 GMT
  host: docs.firstlook.gg
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 12:03:08 2026 GMT
  host: api.firstlook.gg
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pragma Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pragma, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Pragma
provider_slug: pragma
slug: pragma-domain-security
source_filename: pragma-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pragma.gg\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.firstlook.gg\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 22:09:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.firstlook.gg\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 12:03:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: pragma.gg\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: firstlook.gg\n  dnssec: false\n  caa:\n  - ;; connection timed out; no servers could be reached\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pragma/refs/heads/main/security/pragma-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Infrastructure
- Gaming
- Game Backend
- Live Operations
- Player Accounts
- Authentication
- Commerce
- Playtesting
- Community
- Analytics
- Developer Tools
---
