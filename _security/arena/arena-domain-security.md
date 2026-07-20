---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: arena.im
  spf: true
hosts:
- cert_expires: Aug 29 01:16:52 2026 GMT
  host: arena.im
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Arena Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Arena, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Arena
provider_slug: arena
slug: arena-domain-security
source_filename: arena-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: arena.im\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 01:16:52 2026 GMT\n  hsts: false\ndomains:\n- domain: arena.im\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arena/refs/heads/main/security/arena-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Developer Tools
- Audience Engagement
- Live Chat
- Live Blog
- Comments
- Community
- Real-Time
- Moderation
- Media
---
