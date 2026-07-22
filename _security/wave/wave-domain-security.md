---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: wavexr.com
  spf: true
hosts:
- cert_expires: Sep 24 20:05:49 2026 GMT
  host: wavexr.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wave Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wave, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Wave
provider_slug: wave
slug: wave-domain-security
source_filename: wave-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wavexr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 20:05:49 2026 GMT\n  hsts: false\ndomains:\n- domain: wavexr.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wave/refs/heads/main/security/wave-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Entertainment
- Virtual Reality
- Augmented Reality
- Metaverse
- Music
- Live Events
- Avatars
- XR
- Media
---
