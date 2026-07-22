---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: xtool.com
  spf: true
hosts:
- cert_expires: Sep  7 10:03:32 2026 GMT
  host: xtool.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Xtool Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for xTool, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: xTool
provider_slug: xtool
slug: xtool-domain-security
source_filename: xtool-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: xtool.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 10:03:32 2026 GMT\n  hsts: null\ndomains:\n- domain: xtool.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xtool/refs/heads/main/security/xtool-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Technology
- Hardware
- Laser Engraving
- Laser Cutting
- Digital Fabrication
- Manufacturing
- Maker
---
