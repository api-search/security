---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bandcamp.com
  spf: true
hosts:
- cert_expires: Nov 24 22:08:16 2026 GMT
  host: bandcamp.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bandcamp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bandcamp, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bandcamp
provider_slug: bandcamp
slug: bandcamp-domain-security
source_filename: bandcamp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bandcamp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 22:08:16 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: bandcamp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bandcamp/refs/heads/main/security/bandcamp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Music
- Marketplace
- Indie
- Audio
- Sales
- Merch
---
