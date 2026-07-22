---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: fictiv.com
  spf: true
hosts:
- cert_expires: Aug 19 05:30:40 2026 GMT
  host: www.fictiv.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fictiv Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fictiv, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Fictiv
provider_slug: fictiv
slug: fictiv-domain-security
source_filename: fictiv-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fictiv.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 05:30:40 2026 GMT\n  hsts: false\ndomains:\n- domain: fictiv.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fictiv/refs/heads/main/security/fictiv-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Hardware
- Manufacturing
- Digital Manufacturing
- Supply Chain
- CNC Machining
- 3D Printing
- Injection Molding
- Sourcing
- Prototyping
---
