---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: str8bat.com
  spf: true
hosts:
- cert_expires: Sep 11 21:29:35 2026 GMT
  host: str8bat.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Str8Bat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for str8bat, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: str8bat
provider_slug: str8bat
slug: str8bat-domain-security
source_filename: str8bat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: str8bat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 21:29:35 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: str8bat.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/str8bat/refs/heads/main/security/str8bat-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Sports
- Cricket
- IoT
- Sensors
- Wearables
- Analytics
- Sports Technology
- Mobile
---
