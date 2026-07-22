---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: rec.net
  spf: true
hosts:
- cert_expires: Jul 25 21:52:53 2026 GMT
  host: rec.net
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rec Room Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rec Room, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Rec Room
provider_slug: rec-room
slug: rec-room-domain-security
source_filename: rec-room-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rec.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 25 21:52:53 2026 GMT\n  hsts: null\ndomains:\n- domain: rec.net\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rec-room/refs/heads/main/security/rec-room-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Entertainment
- Gaming
- Virtual Reality
- Social Platform
- User Generated Content
- Metaverse
---
