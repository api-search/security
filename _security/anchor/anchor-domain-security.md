---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: anchor.fm
  spf: true
hosts:
- cert_expires: Sep 29 22:42:51 2026 GMT
  host: anchor.fm
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Anchor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Anchor *, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Anchor *
provider_slug: anchor
slug: anchor-domain-security
source_filename: anchor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: anchor.fm\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 29 22:42:51 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\ndomains:\n- domain: anchor.fm\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anchor/refs/heads/main/security/anchor-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Consumer
- Podcasting
- Podcast Hosting
- Audio
- Creator Tools
- Media
- Acquired
---
