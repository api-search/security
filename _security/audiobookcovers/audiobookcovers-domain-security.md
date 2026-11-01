---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: audiobookcovers.com
  spf: true
hosts:
- cert_expires: Jan  9 09:43:13 2027 GMT
  host: audiobookcovers.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Audiobookcovers Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AudiobookCovers, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AudiobookCovers
provider_slug: audiobookcovers
slug: audiobookcovers-domain-security
source_filename: audiobookcovers-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: audiobookcovers.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 09:43:13 2027 GMT\n  hsts: false\ndomains:\n- domain: audiobookcovers.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/audiobookcovers/security/audiobookcovers-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Audiobooks
- CoverArt
- Community
- Free
---
