---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: snapser.com
  spf: false
hosts:
- cert_expires: Oct  3 23:59:59 2026 GMT
  host: snapser.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct  3 23:59:59 2026 GMT
  host: docs.snapser.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Snapser Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Snapser, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Snapser
provider_slug: snapser
slug: snapser-domain-security
source_filename: snapser-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: snapser.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  3 23:59:59 2026 GMT\n  hsts: false\n- host: docs.snapser.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  3 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: snapser.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/snapser/refs/heads/main/security/snapser-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Game Development
- Backend as a Service
- Game Backend
- Authentication
- Leaderboards
- Multiplayer
- Microservices
- SDK Generation
- Developer Tools
---
