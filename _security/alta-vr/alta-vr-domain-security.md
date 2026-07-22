---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: anotheraxiom.com
  spf: false
hosts:
- cert_expires: Sep 11 16:50:44 2026 GMT
  host: www.anotheraxiom.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Alta Vr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alta VR, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Alta VR
provider_slug: alta-vr
slug: alta-vr-domain-security
source_filename: alta-vr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.anotheraxiom.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 16:50:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: anotheraxiom.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alta-vr/refs/heads/main/security/alta-vr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Virtual Reality
- VR
- Gaming
- Game Studio
- Multiplayer
- Social Gaming
- Entertainment
---
