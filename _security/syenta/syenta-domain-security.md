---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: syenta.com
  spf: true
hosts:
- cert_expires: Aug 27 20:06:51 2026 GMT
  host: www.syenta.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Syenta Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Syenta, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Syenta
provider_slug: syenta
slug: syenta-domain-security
source_filename: syenta-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.syenta.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 20:06:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: syenta.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/syenta/refs/heads/main/security/syenta-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Automation
- Semiconductors
- Advanced Packaging
- Chip Manufacturing
- Deep Tech
- Hardware
- AI Infrastructure
---
