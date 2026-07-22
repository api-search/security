---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hellothematic.com
  spf: true
hosts:
- cert_expires: Sep 21 15:55:12 2026 GMT
  host: hellothematic.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Thematic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Thematic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Thematic
provider_slug: thematic
slug: thematic-domain-security
source_filename: thematic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hellothematic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 15:55:12 2026 GMT\n  hsts: false\ndomains:\n- domain: hellothematic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thematic/refs/heads/main/security/thematic-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Music
- Music Licensing
- Content Creators
- Creator Economy
- Copyright
- Royalty-Free Music
- Media
- Audio
---
