---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pocketfm.com
  spf: true
hosts:
- cert_expires: Dec  5 23:59:59 2026 GMT
  host: pocketfm.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pocket Fm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pocket Fm, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Pocket Fm
provider_slug: pocket-fm
slug: pocket-fm-domain-security
source_filename: pocket-fm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pocketfm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: pocketfm.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pocket-fm/refs/heads/main/security/pocket-fm-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Audio
- Streaming
- Audiobooks
- Entertainment
- Media
- Consumer
---
