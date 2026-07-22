---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: kobaltmusic.com
  spf: true
hosts:
- cert_expires: Sep 14 19:18:03 2026 GMT
  host: www.kobaltmusic.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kobaltmusic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kobalt Music, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Kobalt Music
provider_slug: kobaltmusic
slug: kobaltmusic-domain-security
source_filename: kobaltmusic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kobaltmusic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 19:18:03 2026 GMT\n  hsts: false\ndomains:\n- domain: kobaltmusic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kobaltmusic/refs/heads/main/security/kobaltmusic-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Music
- Music Publishing
- Royalties
- Rights Management
- Media
- Entertainment
---
