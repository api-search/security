---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: closingtheory.com
  spf: true
hosts:
- cert_expires: Jan 26 23:59:59 2027 GMT
  host: closingtheory.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Closing Theory Studios Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Closing Theory Studios, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Closing Theory Studios
provider_slug: closing-theory-studios
slug: closing-theory-studios-domain-security
source_filename: closing-theory-studios-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: closingtheory.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: closingtheory.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/closing-theory-studios/refs/heads/main/security/closing-theory-studios-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Gaming
- Mobile Games
- Game Studio
- Real Estate
- Entertainment
- Consumer Apps
---
