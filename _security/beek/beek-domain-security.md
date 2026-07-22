---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: beek.io
  spf: true
hosts:
- cert_expires: Oct 12 05:06:35 2026 GMT
  host: beek.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Beek Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Beek, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Beek
provider_slug: beek
slug: beek-domain-security
source_filename: beek-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: beek.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 05:06:35 2026 GMT\n  hsts: false\ndomains:\n- domain: beek.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beek/refs/heads/main/security/beek-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Intelligent Apps
- Audiobooks
- Media
- Streaming
- Consumer
- Entertainment
- Spanish Language
- Latin America
---
