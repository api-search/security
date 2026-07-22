---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: baton.media
  spf: true
hosts:
- cert_expires: Nov 23 23:59:59 2026 GMT
  host: baton.media
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Baton Media Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Baton Media, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Baton Media
provider_slug: baton-media
slug: baton-media-domain-security
source_filename: baton-media-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: baton.media\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 23 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: baton.media\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/baton-media/refs/heads/main/security/baton-media-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Music
- Music Collaboration
- Creator Economy
- Intellectual Property
- Marketplace
- Audio
- Media
---
